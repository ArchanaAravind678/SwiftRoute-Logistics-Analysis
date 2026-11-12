# SwiftRoute-Logistics-Analysis
An end-to-end Power BI business intelligence solution designed to monitor, analyze, and optimize fleet operations, regional hub efficiency, and driver performance for **SwiftRoute Logistics**.


# 🚚 SwiftRoute Logistics Dashboard

An end-to-end Power BI business intelligence solution designed to monitor, analyze, and optimize fleet operations, regional hub efficiency, and driver performance for **SwiftRoute Logistics**.

---

## 🎯 Problem Statement
SwiftRoute Logistics coordinates daily deliveries across **6 regional hubs**, **55 drivers**, and **45 vehicles**, fulfilling over **1,200 orders per month**. Without centralized, real-time analytics, operations managers faced critical blind spots:
* **Hub Processing Bottlenecks:** Lack of visibility into hub capacity versus incoming order volume led to uneven workloads, with processing times averaging **36.31 hours** and spiking to **40 hours on Fridays**.
* **Suboptimal On-Time Delivery:** With an On-Time Delivery Rate of **77.7%**, leadership struggled to identify which drivers had the highest delay rates or how driver experience influenced service quality.
* **High Fleet Maintenance Downtime:** Over a quarter of the fleet (**26.67% / 12 vehicles**) was inactive due to maintenance, yet managers lacked clear data linking vehicle age, models, and specific vehicle units to recurring breakdowns.

---

## 💡 Complete Solution
To solve these challenges, I developed a 4-page interactive **Power BI Operations Dashboard** that connects hub, driver, and fleet data into a unified reporting system:

### 1. Executive Summary (`SwiftRoute Logistics Dashboard`)
* **KPI Cards with MoM Tracking:** Tracks **Total Orders (1,213)**, **On-Time Delivery Rate (77.7%)**, **CSAT % (82.7%)**, and **Average Delivery Time (36.31 hrs)** against Previous Month (PM) benchmarks.
* **Cross-Functional Overview:** Combines hub capacity, driver performance, and vehicle status onto one screen with one-click navigation buttons to drill into specific operational areas.

### 2. Hubs Overview
* **Capacity vs. Demand Comparison:** Clustered bar charts comparing `Sum of Hub Capacity` against `Total Orders` across Houston, Dallas Main, Austin, San Antonio, Fort Worth, and El Paso.
* **Hub Performance Ranking:** Ranks operational efficiency across hubs, identifying top performers (**Houston Hub at 82.2%**) and laggards (**Fort Worth Hub at 71.7%**).
* **Day-of-Week Processing Heatmap:** Matrix tracking processing hours from Monday to Sunday per hub, pinpointing exact days and locations where delays build up.

### 3. Drivers Overview
* **Dynamic Driver Scorecard:** Interactive dropdown (`DriverName`) showing individual hire dates, Years of Experience (YOE), star ratings, monthly delivery counts (e.g., Christopher Williams with 16 deliveries in March 2024), and a 12-month performance trend line (`Select Measure`).
* **Experience vs. Rating Scatter Plot:** Evaluates how driver tenure correlates with performance ratings.
* **Delay Leaderboard:** Highlights drivers with the highest delay percentages (e.g., Susan Martinez at 45.0% in June; Robert Davis at 41.7% in March) to target coaching.

### 4. Vehicle Overview
* **Fleet Status Tracker:** Donut chart monitoring active vs. maintenance vehicles (**33 Active** vs. **12 in Maintenance**).
* **Breakdown Root-Cause Analysis:**
  * *Vehicle Age vs. Breakdown:* Scatter plot proving breakdown frequency rises sharply as vehicles age past 6–8 years.
  * *Breakdown by Model & Code:* Identifies top breakdown models (**Freightliner M2 with 153 breakdowns**) and specific high-risk units (**FT-010 with 28 breakdowns**).
* **Order Volume by Vehicle Type & Model:** Breaks down order fulfillment by vehicle class (**Vans leading at 62.82% / 762 orders**, followed by Trucks at 22.18%).

---

## 🔍 Key Insights & Actionable Recommendations

| Operational Area | Key Data Insight | Business Recommendation |
| :--- | :--- | :--- |
| **Hub Operations** | Order processing peaks at **40 hours on Fridays**, and **Fort Worth Hub** trails in performance at **71.7%**. | Reallocate Thursday/Friday shift staff at San Antonio and Houston hubs (38-hr averages) and audit Fort Worth workflows to match Houston's 82.2% benchmark. |
| **Fleet Management** | **26.67%** of vehicles are in maintenance, with breakdowns heavily concentrated in **6–8+ year-old vehicles** and the **Freightliner M2** model (153 breakdowns). | Schedule preventative maintenance for high-breakdown units (`FT-010`, `FT-002`) and initiate a phased replacement plan for aging Freightliner M2 trucks. |
| **Driver Performance** | Certain drivers show delay rates above **38%–45%** despite strong overall CSAT (**82.7%**). | Pair high-delay drivers with experienced mentors and review route assignments on congested corridors to lift On-Time Delivery above 85%. |
| **Fleet Utilization** | **Vans** handle **62.82%** of all orders, outperforming Trucks (22.18%) and Pickups (9.98%). | Expand the Van fleet during peak months (May–June) to maximize delivery throughput and fuel efficiency. |

---

## 🛠️ Tech Stack & Skills Demonstrated
* **BI & Visualization:** Microsoft Power BI Desktop
* **Data Modeling & DAX:** Time Intelligence (`Previous Month` variance), dynamic measure selection, conditional formatting heatmaps, and KPI cards.
* **Dashboard UX/UI:** Custom sidebar navigation, cross-page filtering via `Year` and `Month` slicers, and intuitive visual hierarchy.

---

## 🚀 How to Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Open `SwiftRoute_Logistics_Dashboard.pbix` in **Power BI Desktop**.
3. Use the left-hand navigation menu to explore **Executive Summary**, **Drivers Overview**, **Hubs Overview**, and **Vehicle Overview**, and filter by **Year** and **Month**.

