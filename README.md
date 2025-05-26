# Power BI Transportation & Logistics Analysis - Portfolio Showcase 

##  Project Introduction

This project showcases a comprehensive Power BI dashboard designed for in-depth analysis and actionable insights into transportation and logistics operations for "LOGO" *(or "a leading [Industry] company")*. The primary objective was to transform raw operational data into actionable intelligence, enabling stakeholders to effectively monitor costs, evaluate vendor performance, optimize in-house fleet efficiency, and make informed, data-driven strategies for optimization and cost reduction within a dynamic supply chain environment.

The dashboard moves beyond simple reporting, offering interactive visualizations and drill-through capabilities to explore the nuances of transportation data, identify key trends, and pinpoint areas for operational improvement.

---

##  Key Dashboard Objectives & Business Value

*   ** Cost Visibility & Control:** To gain a transparent view of total transportation expenditures, broken down by various dimensions such as time, geographical region, payload capacity, and service provider.
*   ** Vendor Performance Management:** To rigorously evaluate and benchmark the performance of external transportation vendors based on cost-effectiveness (e.g., overall cost, cost per trip, cost per CBM/KM) and operational efficiency (e.g., load factor).
*   ** In-house Fleet Optimization:** To analyze the productivity and efficiency of the internal fleet, with a keen focus on driver performance metrics (total trips, distance, active days, load utilization, trips per active day) and vehicle usage patterns.
*   ** Identification of Inefficiencies & Opportunities:** To proactively identify high-cost areas, underperforming vendors or drivers, and opportunities for improving load consolidation or resource allocation.
*   ** Strategic Decision Support:** To furnish a robust analytical foundation for strategic initiatives, including vendor negotiations, fleet management adjustments, and overall logistics strategy refinement.

---

##  Dashboard Structure & Core Features

The dashboard suite is comprised of an Overview page, a Vendor analysis page, an In-house fleet analysis page, and a drill-through Driver Detail page, each tailored for specific analytical insights. All pages are highly interactive, featuring dynamic filtering and custom tooltips for enhanced data exploration.

### 1. Overview Page: Holistic Performance Snapshot 

*This page provides a high-level summary of the entire transportation operation, allowing for quick assessment of key trends and figures.*

![Overview Page](![Overview Page](https://github.com/user-attachments/assets/179abc74-68ab-4136-9a9f-627ad851f3d6)
) 
*(Ensure this image path is correct and the image is fully anonymized. The red/teal from this image will be key.)*

*   **Key Performance Indicators (KPIs):**
    *   Total Transportation Cost (e.g., "1000 bnđ") with YoY % change.
    *   Total Trips (e.g., "1000") with YoY % change.
    *   Average Cost per CBM (e.g., "1000") with YoY % change.
    *   Average Cost per KM (e.g., "1000") with YoY % change.
*   **Cost & Operational Breakdowns:**
    *   Cost by Payload *(Clarify X-axis labels in your description if they are just numbers, e.g., "Cost by Payload Capacity (Tons)").*
    *   Total Trips by Province *(Address any "(Blank)" entries).*
    *   Cost/CBM by Province.
    *   Load Factor by Province (%).
*   **Trend Analysis (Time Series):**
    *   Average Load Factor (%) Over Time (2020-2025).
    *   Total Cost (Billion VND) Over Time (2020-2025) *(Note any forecasts, e.g., for 2025).*
*   **Geospatial Analysis:**
    *   Total Cost by Province (Map) *(Mention if a legend is present or what colors signify).*
*   **Interactive Elements:** Slicers for Year, Province, Payload; "RESET" button; Custom Report Page Tooltip for map.
    ```markdown
    ![Overview Map Tooltip](![Tool Tips Province](https://github.com/user-attachments/assets/ea3ad93f-374a-4ed8-84ec-5fa06f1f5993)
) 
    ```

### 2. Vendor Analysis Page: Managing Partner Performance 📈

*This page focuses on a detailed evaluation and comparison of third-party logistics providers.*

![Vendor Page](![Vendor Page](https://github.com/user-attachments/assets/fa9e8ebd-45d4-4cd5-9240-ad8eef42134d)
)

*   **Vendor-Specific KPIs:** Total Vendor Cost, Number of Active Vendors, Overall Avg Cost Per Trip, Overall Average Load Factor *(Clarify calculation method for overall averages).*
*   **Vendor Contribution & Ranking:** Total Cost By Vendor (Top N + "Others"), Total Trips By Vendor (Top N + "Others").
*   **Comparative Vendor Performance Charts:** Avg Cost Per Trip by Vendor, Avg Cost Per CBM by Vendor *(Strongly recommend adding overall average reference lines to these charts in your actual dashboard and mentioning it here).*
*   **Detailed Vendor Performance Table:** Key metrics per vendor (`% Total Cost`, `Total Trips`, `Avg % Load`, `Avg Cost Per Trip`, `Avg Cost Per CBM`). *Ensure "Total" row calculations are accurate overall figures.*
*   **Vendor Cost Trend Analysis:** Line chart for key vendors' cost trends (2022-2025).
*   **Interactive Elements:** Slicers; Custom Tooltip for vendor details.
    ```markdown
    ![Vendor Detail Tooltip](![Tool tips Vendor](https://github.com/user-attachments/assets/c72e8b0f-f285-4261-8a50-0b44e3db947b)
)
    ```

### 3. In-house Fleet Analysis Page: Optimizing Internal Resources 🛠️

*This page is dedicated to analyzing the efficiency and productivity of the company-owned/operated fleet and its drivers.*

![Inhouse Page](![Inhouse Page](https://github.com/user-attachments/assets/34957d29-b8bc-4224-b647-4c422c24ac9e)
)

*   **In-house Fleet KPIs:** Total Trips, Total Distance (specify unit), Avg Trip/Driver, Total Driver Active Days (all with YoY % change).
*   **Driver & Vehicle Performance Breakdown:**
    *   Total Trips by In-house Payload Capacity.
    *   Top 5 Drivers by Total Distance.
    *   Load Factor By In-house Payload Type *(Clarify X-axis payload labels if codes).*
    *   Top 5 Drivers by Active Days.
    *   **Driver Performance Scatter Plot:** `Total Trips` vs. `Average Trip Distance` (or `Total Distance` - *clarify X-axis*) with average reference lines for quadrant analysis.
*   **Detailed Driver Performance Table:** `Driver Name`, `Total Trips`, `Active Days`, `Avg % Load`, `Total Distance`, `Avg Trips per Active Day`.
*   **Interactive Elements:** Slicers; "RESET" button; Drill-through to "Driver Detail" page; Custom Tooltip for scatter plot.
    ```markdown
    ![Inhouse Driver Scatter Tooltip](![Tool Tips Driver](https://github.com/user-attachments/assets/8479988e-f079-4e4e-8457-41a99f79cf7e)
)
    ```

### 4. Drill Through Driver Detail Page 👨‍✈️👩‍✈️

*This dedicated page provides an in-depth look at the performance and activity trends of a single, selected driver.*

![Drill Through Driver Detail Page](![Drill Through Driver Detail](https://github.com/user-attachments/assets/4ec59d5b-c9e2-49d5-aef9-9ed09cac4833)
)

*   **Selected Driver's KPIs:** Prominently displays `Driver Name` with their specific KPIs.
*   **Monthly Performance Trends:** Combined Column/Line chart for `Avg Trips/Driver` & `Total Distance`; Line chart for `Avg % Load Factor`.
*   **Recent Trips Table:** Details of last 5 trips (`Date`, `Cargo Details`, `Vehicle Details`, `Distance`, `% Load`). *(Clarify any unclear column headers like "Khối hàng").*
*   **Trip Characteristic Breakdown:** Pie chart for "Average of % Load" (could be "Trip Distribution by % Load Factor Bins").

---

##  Technical Skills & Tools Utilized

*   **Primary Tool:** Microsoft Power BI Desktop
*   **Data Transformation (Power Query / M Language):**
    *   Connected and integrated data from diverse sources (e.g., Excel files, CSVs).
    *   Performed comprehensive data cleaning, preprocessing, and shaping (handling missing values, standardizing formats, merging/appending queries, creating custom/conditional columns).
*   **Data Modeling:**
    *   Designed and implemented a relational data model (Star Schema) with Fact and Dimension tables (`Dim_Date`, `Dim_Vendors`, `Dim_Drivers`, etc.).
    *   Established and managed table relationships.
    ```markdown
    ![Data Model Diagram (Anonymized)](images/data_model_anonymized.png) 
    ```
*   **DAX (Data Analysis Expressions):**
    *   Authored numerous complex DAX measures for dynamic KPIs (YoY changes, averages, percentages, Top N, conditional aggregations).
    *   Utilized key DAX functions: `CALCULATE`, `SUMX`, `AVERAGEX`, `DIVIDE`, `FILTER`, `ALL`, `ALLEXCEPT`, `VALUES`, `DISTINCTCOUNT`, `SAMEPERIODLASTYEAR`, `IF`, `SWITCH`, `TOPN`.
    *   Created Calculated Columns for categorization (e.g., Load Factor Bins).
*   **Data Visualization & Dashboard Design:**
    *   Employed a variety of appropriate visuals (Column, Line, Scatter, Map, Table, KPI Cards, Slicers).
    *   Focused on an intuitive UI/UX with consistent branding (leveraging the "Sunhouse red" and "teal" from dashboard visuals).
    *   Implemented advanced interactive features: Custom Report Page Tooltips, Drill-through, Slicers, Cross-filtering, "RESET" button.
    *   Applied Conditional Formatting for visual highlighting.

---
*(Optional: Insert a simple red or teal banner image here if you create one)*
---

##  Key Analytical Insights & Outcomes (Illustrative)

> This dashboard empowers users to:
> *    Identify cost hotspots by province or payload type.
> *    Benchmark vendor efficiency on unit costs and load utilization.
> *    Profile driver productivity based on volume, distance, active days, and load efficiency.
> *    Classify drivers into performance segments using the scatter plot for targeted actions.
> *    Track performance trends over time to detect anomalies or improvements.
> *    Provide data-backed evidence for vendor negotiations and fleet management.

---

##  Conclusion & Potential Future Enhancements

This Power BI Transportation Analysis dashboard serves as a robust analytical tool, transforming complex logistics data into clear, actionable insights. It is designed to be a critical asset for operational monitoring, strategic planning, and continuous improvement in transportation management.

**Potential future enhancements could include:**

*   Detailed In-house Fleet Costing.
*   On-Time Delivery (OTD) Tracking.
*   Predictive Analytics for costs and demand.
*   Route Optimization Analysis.

---

## <a name="data-privacy"></a> Important Note on Data Privacy & Project Sharing

The Power BI project file (.pbix) for this dashboard is **not shared publicly** in this repository. This decision is due to the dashboard's original connection to confidential and proprietary company data.

The screenshots and descriptions provided herein showcase the dashboard's structure, design, analytical capabilities, and the technical skills employed in its development. All sensitive data within these visuals has been **anonymized, replaced with sample data, or obscured** to rigorously protect company information and ensure confidentiality.

The primary purpose of this portfolio piece is to demonstrate my proficiency in Power BI development, data modeling, DAX, and dashboard design for logistics and transportation analysis. I am enthusiastic about discussing the methodologies, technical challenges, and specific DAX solutions implemented in this project in more detail during an interview.

---

##  Contact

*   **LinkedIn:** `[Your LinkedIn Profile URL]`
*   **Email:** `[Your Email Address]`
*   **(Optional) Portfolio Website:** `[Your Portfolio Website URL]`
