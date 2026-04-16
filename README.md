# deloitte-tableau-analysis
# Daikibo Telemetry Data Analysis (Tableau)

## 📊 Overview
This project analyzes machine telemetry data from Daikibo’s 4 factories for the month of May 2021.

Each factory operates 9 types of machines that send status updates every 10 minutes. The goal of this analysis was to identify:
- Which factory experienced the most machine breakdowns
- Which machine types contributed most to downtime in that factory

---

## 🎯 Objectives
- Determine the factory with the highest downtime
- Identify the most failure-prone machine types within that factory
- Build an interactive dashboard to visualize downtime patterns

---

## 🛠 Tools Used
- Tableau Desktop
- JSON data (telemetry dataset)

---

## 🧹 Data Preparation
- Imported and parsed nested JSON data into Tableau
- Ensured all schema levels were correctly expanded
- Created a calculated field:

**Unhealthy (Calculated Measure):**
- Assigned a value of 10 for each "unhealthy" status
- Represents 10 minutes of downtime per event

---

## 📈 Visualizations

### 1. Down Time per Factory
- Bar chart showing total downtime across all 4 factories

### 2. Down Time per Device Type
- Bar chart showing downtime by machine type
- Dynamically filtered based on selected factory

---

## 📊 Dashboard Features
- Interactive dashboard combining both charts
- Factory selection acts as a filter
- Enables drill-down into machine performance per location

---

## 🔍 Key Insights
- The factory with the highest downtime was: Daikibo Factory Seiko
- The machines contributing most to failures were:
  - LaserWelder
- Downtime patterns suggest potential maintenance or operational inefficiencies in this location

---

## 📁 Files in this Repository
- `daikibo-dashboard.twbx` – Tableau packaged workbook
- `dataset.json` – Raw telemetry data (if included)
- `images/` – Dashboard screenshots

---

## ▶️ How to View
1. Download the `.twbx` file  
2. Open using Tableau Desktop  
3. Interact with the dashboard filters to explore insights  

---

## 📸 Dashboard Preview
![Dashboard](dashboard.png)

---

## ⚠️ Notes
- This project is based on a simulated business case
- No sensitive or real company data is exposed
