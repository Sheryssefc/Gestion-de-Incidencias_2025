# Gestion-de-Incidencias_2025
Dashboard interactivo en Power BI para gestión de incidencias | Power Query, DAX, ETL | Caso demostrativo

# Jira Incident Report - FinanSmart (2025)
Interactive dashboard developed in Power BI for monitoring and analyzing technical support requests, with **emphasis on SLA compliance**. This project simulates an incident management system for a fictional company, based on real experience in ticket management.

## Objective
Develop an executive dashboard **focused on SLA monitoring** (Service Level Agreement) as a critical metric, additionally enabling:
- **Prioritize SLA compliance tracking** as the main metric
- Visualize request volume and status
- Analyze support team performance
- Identify recurring problem areas
- Optimize resource allocation by request type

## Key Metrics
- **562** total requests
- **89.15%** of tickets resolved
- **SLA compliance** tracking
- Distribution by **request type** (Hardware, Software, VPN, etc.)
- Workload analysis by **assignee**
- Historical trend by **month and year**

## Data Loading Process in Power BI

### 1. Data Collection
- Export data from ticket system (CSV format)
- Organize by status, problem type, and responsible person

### 2. Data Cleaning & Transformation
- **Grammar correction** in textual data
- **Remove redundant words** to improve analysis quality
- **Eliminate incomplete records** to ensure accuracy
- **Data type conversion** (dates, numbers,  text)

#### Critical SLA Transformation:
- **"Time to Resolution" field:** Conversion of hour format to recognizable standard
- **SLA compliance calculation:** Transformation to binary metric (**Yes/No**) based on time limits
- **"SLA_Compliance" column creation:** Automatic classification using Power Query
- **Consistency validation** in resolution times

### 3. Visualization Creation
- **Import to Power BI** from CSV files
- **Transform fields** to appropriate formats
- **Interactive dashboard** with bar charts, line graphs, and KPI cards
- **SLA visualization** as main metric with clear indicators
- **Area analysis** to identify zones with the most problems

### 4. Filters & Metrics
- **Interactive filters** by month, responsible person, and problem type
- **Custom KPI measures** for calculating total incidents by status
- **Average resolution time** and other key metrics

## Dashboard Views

### Overall Dashboard
![Complete Dashboard](captura-dashboard-completo.png)
*Complete dashboard view with all main metrics and visualizations*

### Monthly Analysis (October 2025)
![Filter by Month](captura-mes-octubre.png)
*Filtered by October 2025: shows monthly request distribution and **temporal SLA compliance trends***

### Performance by Assignee
![Filter by Person](captura-persona-asignada.png)
*Workload analysis by team member and **SLA compliance efficiency***

### Diagnosis by Incident Type
![Filter by Incident](captura-incidencia.png)
*Segmentation by specific incident type to identify **problems affecting SLA***

### Distribution by Request Type
![Filter by Request](captura-tipo-solicitud.png)
*Categorized analysis by request type (Hardware, Software, VPN, DB Access, etc.)for **optimizing specialized resource allocation** and **anticipating infrastructure needs**.*


## Business Impact
- **Improved incident response**: Analysis helps team respond faster to recurring problems
- **Critical area prioritization**: Identification of zones with highest incident volume
- **Data-driven decisions**: Implementation of improvements in high-volume areas
- **Immediate SLA compliance visibility** for management decision-making
- **Resource optimization** based on recurring request types and patterns
- **Proactive monitoring** of service level agreement breaches

## Technology Stack
- **Power BI** for visualization and dashboards
- **Power Query** for data transformation and cleaning (ETL) - **including critical SLA time transformation**
- **DAX** for creating custom metrics
- **Excel/CSV** as data source

## How to Use the Dashboard
The dashboard allows:
1. **Monitor SLA compliance** as main metric
2. **Filter by month** for trend analysis
3. **Select assignee** for individual SLA performance evaluation
4. **Filter by incident type** for specific diagnosis
5. **Analyze by request type** for resource optimization

---

*Note: The data used is fictional and created for professional demonstration, based on real experience in incident management with SLA focus. The dashboard logo, while simple, was personally created for this project.*
