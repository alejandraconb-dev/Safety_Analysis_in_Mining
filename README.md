# Safety_Analysis_in_Mining
En el sector minero, la gestión de eventos de seguridad y salud ocupacional (HSS), que incluye observaciones, casi accidentes (near misses) e incidentes, requiere visibilidad oportuna para prevenir accidentes. Se disponía de 3 archivos CSV con datos de eventos HSS, colaboradores (reportantes y dueños de acciones) y una dimensión calendario, pero los datos presentaban problemas de calidad: la columna de semanas venía completamente vacía, había inconsistencias en formatos de texto y faltaba un dashboard que consolidara indicadores clave para la toma de decisiones por parte de perfiles gerenciales y de operaciones.

## Descripción del proyecto

Este proyecto consiste en la construcción de un panel de control (dashboard) de una página que permite monitorear eventos de seguridad y las acciones correctivas asociadas.

El objetivo principal es entregar información clara y accionable para usuarios no técnicos (gerencias, superintendencias y equipos de HSS), facilitando la identificación de:
- Volumen de eventos
- Eventos aún abiertos
- Acciones vencidas
- Distribución por área y nivel de riesgo

## Fuentes de datos

Se utilizaron 4 archivos CSV:

| Archivo            | Descripción                                      |
|--------------------|--------------------------------------------------|
| `events.csv`       | Eventos de seguridad (observaciones, near miss, incidentes, etc.) |
| `actions.csv`      | Acciones asociadas a los eventos                 |
| `employees.csv`    | Colaboradores (reportantes y dueños de acciones) |
| `dim_date.csv`     | Dimensión de calendario                          |

## Proceso realizado

1. **Limpieza y preparación de datos** (Python / Pandas en Google Colab)
   - Manejo de valores nulos
   - Normalización de textos
   - Corrección de formatos de fecha
   - Cálculo de la columna `Week` en la dimensión de fecha
   - Eliminación de duplicados

2. **Modelado de datos en Power BI**
   - Relaciones entre eventos, acciones, empleados y calendario
   - Creación de medidas DAX para los KPIs

3. **Visualización**
   - Diseño orientado a usuarios no técnicos
   - Uso de colores con significado (alerta y semáforo de riesgo)
   - Títulos claros y jerarquía visual simple

## KPIs principales

- **Total de Eventos**
- **Eventos Abiertos**
- **Total de Acciones**
- **Acciones Vencidas** (acciones no completadas cuya fecha de vencimiento ya pasó)

## Visualizaciones incluidas

- Acciones vencidas por área
- Eventos por área
- Distribución de eventos por nivel de riesgo (gráfico circular)

## Cómo usar este repositorio

1. Descarga el archivo `.pbix` (o el enlace al reporte publicado en Power BI Service).
2. Ábrelo con Power BI Desktop o visualízalo directamente en Power BI Service.
3. Utiliza los filtros de Fecha, Sitio, Área y Nivel de Riesgo para explorar los datos.

## Herramientas utilizadas

- Google Colab + Pandas (limpieza de datos)
- Power BI Service (modelado y visualización)
- DAX (medidas)


### Consejos rápidos para GitHub

- Sube el archivo `.pbix` (o un enlace si es muy pesado).
- Si quieres, agrega una carpeta `/data` con los CSV limpios (sin datos sensibles).
- Puedes poner una captura del dashboard final en la parte superior del README (se ve mucho más profesional).

¿Quieres que te prepare también una versión más corta del README o una sección de “Hallazgos principales”?
