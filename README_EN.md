<img src="https://github.com/alejandraconb-dev/Safety_Analysis_in_Mining/blob/main/grafico_hss.png" width="5000"> 

# 📌Safety_Analysis_in_Mining
In the mining sector, the management of occupational health and safety (HSS) events, which includes observations, near misses and incidents, requires timely visibility to prevent accidents.
## 📎 Description of the project

This project consists of the construction of a one-page dashboard that allows to monitor security events and the associated corrective actions.

The main objective is to provide clear and actionable information for non-technical users (managers, superintendencies and HSS teams), facilitating the identification of:
- Volume of events.
- Events still open.
- Expired shares.
- Distribution by area and level of risk.

## 🖥️Tools used

- Power BI Desktop and Service (modeling and visualization).
- DAX (measures).
  
## Data sources

4 CSV files were used:

| Archive            | Description                                   |
|--------------------|--------------------------------------------------|
| `events.csv`       | Security events (observations, near misses, incidents, etc.) |
| `actions.csv`      | Actions associated with the events               |
| `employees.csv`    | Collaborators (reporters and owners of shares) |
| `dim_date.csv`     | Calendar dimension                          |

## Process carried out

1. **Data cleaning and preparation**
   - Handling of null values.
   - Standardization of texts.
   - Correction of date formats. 
   - Calculation of the  `Week` column in the date dimension.
   - Elimination of duplicates.

2. **Data modeling in Power BI**
   - Relationships between events, actions, employees and calendar.
   - Creation of DAX measures for KPIs.

## 📈Main KPIs

- **Total de Eventos** (Total of Events).
- **Eventos Abiertos** (Open Events).
- **Total de Acciones**.
- **Acciones Vencidas** (acciones no completadas cuya fecha de vencimiento ya pasó).

##  📊Visualizaciones incluidas

- Acciones vencidas por área.
- Eventos por área.
- Distribución de eventos por nivel de riesgo (gráfico circular).

##  ▶️ Cómo usar este repositorio

1. Download the file `.pbix` (or the link to the report published in Power BI Service).
2. Open it with Power BI Desktop or view it directly in Power BI Service.
3. Use the Date, Site, Area and Risk Level filters to explore the data.
<img src="https://github.com/alejandraconb-dev/Safety_Analysis_in_Mining/blob/main/dashboardseguridadhss.GIF" width="5000">

</br>

💙 <strong>Alejandra Contreras</strong> :octocat: </br></br>
<a href="https://www.linkedin.com/in/alejandraconb-dev/" target="_blank">
<img align="left" src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
<img align="center" src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Smilies/Relieved%20Face.png" target="_blank" height="40"></a>
