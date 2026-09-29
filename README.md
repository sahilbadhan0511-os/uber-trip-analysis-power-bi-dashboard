# 🚕 Uber Trip Analysis Dashboard | Power BI

An interactive **Uber Trip Analysis Dashboard** developed using **Microsoft Power BI** to analyze trip bookings, booking value, trip distance, vehicle types, pickup locations, and time-based travel patterns.

The project demonstrates practical skills in **Data Analytics, Data Visualization, Power BI, DAX, Data Modeling, KPI Analysis, and Dashboard Development**.

---

## 📊 Project Overview

The objective of this project is to analyze Uber trip data and create an interactive dashboard that helps users understand:

* Total number of bookings
* Total booking value
* Total trip distance
* Average booking value
* Average trip distance
* Trip trends over time
* Vehicle type performance
* Pickup location performance
* Booking patterns
* Revenue patterns
* Distance-based trip analysis

The dashboard allows users to interact with the data using filters and visualizations.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze Uber trip and booking data.
2. Identify important business KPIs.
3. Analyze booking and revenue trends.
4. Study trip distance patterns.
5. Compare different vehicle types.
6. Identify frequently used pickup locations.
7. Analyze trips based on time.
8. Create an interactive Power BI dashboard.
9. Implement DAX measures for dynamic analysis.
10. Provide useful insights through data visualization.

---

## 🛠️ Tools & Technologies

| Technology         | Purpose                          |
| ------------------ | -------------------------------- |
| Microsoft Power BI | Dashboard development            |
| Power Query        | Data cleaning and transformation |
| DAX                | Calculated measures and KPIs     |
| Microsoft Excel    | Data storage and preprocessing   |
| Data Modeling      | Relationships between tables     |
| Data Visualization | Charts and interactive reports   |

---

## 📁 Dataset

The project uses Uber trip-related data containing information such as:

* Trip ID
* Date
* Time
* Booking value
* Trip distance
* Vehicle type
* Pickup location
* Drop location
* Booking status
* Payment information
* Customer/trip-related attributes

A separate location table is used for location-based analysis.

---

# 📈 Dashboard Pages

The Power BI report contains multiple analytical pages.

## 1. Overview

The **Overview** page provides a high-level summary of Uber trip performance.

### Key KPIs

* Total Bookings
* Total Booking Value
* Total Trip Distance
* Average Booking Value
* Average Trip Distance

### Main Analysis

The Overview page can be used to analyze:

* Booking performance
* Revenue performance
* Trip distance
* Vehicle category
* Pickup locations
* Overall trip distribution

---

## 2. Time Analysis

The **Time Analysis** page focuses on time-based patterns.

It can be used to understand:

* Daily booking trends
* Monthly booking trends
* Hourly booking patterns
* Revenue trends
* Trip distance trends
* Peak travel periods

This analysis helps identify periods with higher or lower trip activity.

---

## 3. Details

The **Details** page is designed as a drill-through analysis page.

It provides detailed information related to selected KPIs such as:

* Total Booking Value
* Total Bookings
* Total Trip Distance

Users can move from high-level dashboard analysis to more detailed information.

---

# 📊 Key Metrics

Important metrics used in the dashboard include:

### Total Bookings

Measures the total number of Uber bookings.

```DAX
Total Bookings =
COUNT('Trip Details'[Trip ID])
```

---

### Total Booking Value

Calculates the total value of all bookings.

```DAX
Total Booking Value =
SUM('Trip Details'[Booking Value])
```

---

### Total Trip Distance

Calculates the total distance travelled.

```DAX
Total Trip Distance =
SUM('Trip Details'[Trip Distance])
```

---

### Average Booking Value

```DAX
Average Booking Value =
AVERAGE('Trip Details'[Booking Value])
```

---

### Average Trip Distance

```DAX
Average Trip Distance =
AVERAGE('Trip Details'[Trip Distance])
```

---

## 🧹 Data Preparation

The following data preparation steps were performed using Power Query:

1. Imported the Uber dataset.
2. Checked column names and data types.
3. Removed unnecessary columns.
4. Handled missing values.
5. Corrected data types.
6. Standardized date and time fields.
7. Checked duplicate records.
8. Created/used a location table.
9. Created relationships between tables.
10. Loaded the cleaned data into Power BI.

---

# 🔗 Data Model

The project uses a relational data model involving the trip data and location information.

Example model:

```text
              ┌─────────────────────┐
              │    Location Table    │
              │                     │
              │ Location            │
              │ Location ID         │
              └──────────┬──────────┘
                         │
                         │
                         ▼
              ┌─────────────────────┐
              │    Trip Details     │
              │                     │
              │ Trip ID             │
              │ Booking Value       │
              │ Trip Distance       │
              │ Pickup Location     │
              │ Drop Location       │
              │ Vehicle Type        │
              │ Date                │
              │ Time                │
              └─────────────────────┘
```

---

# 📌 DAX

DAX was used to create dynamic measures for dashboard analysis.

Examples:

```DAX
Total Bookings =
COUNT('Trip Details'[Trip ID])
```

```DAX
Total Booking Value =
SUM('Trip Details'[Booking Value])
```

```DAX
Total Trip Distance =
SUM('Trip Details'[Trip Distance])
```

```DAX
Average Booking Value =
AVERAGE('Trip Details'[Booking Value])
```

```DAX
Average Trip Distance =
AVERAGE('Trip Details'[Trip Distance])
```

Additional DAX measures can be found in the `DAX/Measures.md` folder.

---

# 📊 Dashboard Features

The dashboard includes:

* Interactive KPI cards
* Time-based analysis
* Vehicle type analysis
* Booking analysis
* Revenue analysis
* Distance analysis
* Pickup location analysis
* Interactive filters
* Drill-through analysis
* Dynamic Power BI visuals
* Data-driven insights

---

# 🔍 Business Questions

The dashboard can help answer questions such as:

### Booking Analysis

* How many trips were completed?
* Which periods have the highest number of bookings?
* How does booking volume change over time?

### Revenue Analysis

* What is the total booking value?
* Which periods generate higher booking value?
* What is the average booking value?

### Distance Analysis

* What is the total distance travelled?
* What is the average trip distance?
* How does trip distance vary across vehicle types?

### Location Analysis

* Which locations have the highest pickup activity?
* Which locations have lower trip activity?
* How are trips distributed across locations?

### Vehicle Analysis

* Which vehicle types are used most frequently?
* How does booking value vary by vehicle type?
* How does trip distance vary by vehicle type?

---

# 💡 Key Skills Demonstrated

This project demonstrates practical knowledge of:

### Data Analytics

* Data cleaning
* Data transformation
* Exploratory analysis
* KPI analysis
* Trend analysis

### Power BI

* Power Query
* Data modeling
* Relationships
* Visualizations
* Filters
* Slicers
* Drill-through
* Dashboard design

### DAX

* SUM
* COUNT
* AVERAGE
* CALCULATE
* FILTER
* TOPN
* SUMMARIZE
* CONCATENATEX
* Dynamic measures

---

# 🚀 Project Workflow

```text
Raw Uber Dataset
       ↓
Data Cleaning
       ↓
Data Transformation
       ↓
Power Query
       ↓
Data Modeling
       ↓
DAX Measures
       ↓
Data Visualization
       ↓
Interactive Dashboard
       ↓
Business Insights
```

---

# 📷 Dashboard Preview

Add screenshots of your Power BI dashboard in the `Dashboard` folder.

Example:

```markdown
## Dashboard Preview

![Overview Dashboard](Dashboard/Overview.png)

![Time Analysis](Dashboard/Time_Analysis.png)

![Details Dashboard](Dashboard/Details.png)
```

---

# ▶️ How to Use

1. Download or clone this repository.
2. Install Microsoft Power BI Desktop.
3. Open:

```text
PowerBI/Uber_Trip_Analysis.pbix
```

4. If required, update the dataset path in Power Query.
5. Refresh the data.
6. Explore the dashboard using filters and interactive visuals.

---

# 📂 Repository Structure

```text
uber-trip-analysis-powerbi-dashboard
│
├── README.md
│
├── PowerBI
│   └── Uber_Trip_Analysis.pbix
│
├── Dataset
│   ├── Uber_Trip_Details.xlsx
│   └── Location_Table.xlsx
│
├── Dashboard
│   ├── Overview.png
│   ├── Time_Analysis.png
│   └── Details.png
│
├── DAX
│   └── Measures.md
│
└── Documentation
    ├── Data_Model.png
    └── Project_Documentation.pdf
```

---

# 🎓 Academic / Portfolio Use

This project was developed as a **Data Analytics and Business Intelligence portfolio project** using Microsoft Power BI.

It demonstrates the complete analytics workflow from data preparation to interactive dashboard development.

---

# 👨‍💻 Author

**Sahil Pankaj Badhan**

B.E. Information Technology Engineering Student

### Skills

* Python
* SQL
* Excel
* Power BI
* Tableau
* Data Analytics
* Data Visualization
* Machine Learning
* Artificial Intelligence




