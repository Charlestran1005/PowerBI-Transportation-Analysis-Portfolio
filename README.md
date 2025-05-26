# Power BI Transportation & Logistics Analysis - Portfolio Showcase

## Project Introduction

This project presents a comprehensive Power BI dashboard developed to provide in-depth analysis and actionable insights into transportation and logistics operations. The primary objective was to transform raw operational data into strategic intelligence, enabling stakeholders to effectively monitor costs, evaluate vendor performance, optimize in-house fleet efficiency, and make informed, data-driven decisions to enhance the supply chain.

The dashboard suite moves beyond static reporting, offering a dynamic and interactive experience with multiple interconnected pages, advanced visualizations, custom tooltips, and drill-through capabilities to explore the nuances of transportation data, identify key trends, and pinpoint areas for operational improvement.

---

## Key Dashboard Objectives & Business Value

*   **Comprehensive Cost Visibility & Control:** To gain a transparent, multi-dimensional view of total transportation expenditures, segmented by time, geographical region, payload capacity, and service provider.
*   **Strategic Vendor Performance Management:** To rigorously evaluate and benchmark the performance of external transportation vendors based on cost-effectiveness (e.g., total cost contribution, average cost per trip, average cost per CBM) and operational efficiency (e.g., % load factor).
*   **In-house Fleet Optimization & Productivity:** To analyze the productivity and efficiency of the internal fleet, with a keen focus on driver performance metrics (total trips, distance covered, active operational days, load utilization, and average trips per active day) and vehicle usage patterns.
*   **Proactive Identification of Inefficiencies & Opportunities:** To identify high-cost routes or regions, underperforming vendors or drivers, and opportunities for improving load consolidation, resource allocation, or route planning.
*   **Data-Driven Strategic Decision Support:** To furnish a robust analytical foundation for strategic initiatives, including vendor contract negotiations, fleet management adjustments, network design considerations, and overall logistics strategy refinement.

---

## Dashboard Structure & Core Features

The dashboard is structured into several key analytical pages: Overview, Vendor Analysis, In-house Fleet Analysis, and a detailed Drill-Through Driver Detail page. Each page is designed for specific insights and features dynamic filtering and custom tooltips for an enhanced data exploration experience.

### 1. Overview Page: Holistic Performance Snapshot

*This page provides a high-level "control tower" view of the entire transportation operation, enabling quick assessment of key trends and headline figures.*

![Overview Page](https://github.com/user-attachments/assets/6be3a411-b0ed-4869-b0e0-2afe3d3f2146)



*   **Key Performance Indicators (KPIs):**
    *   **Total Cost:** Overall transportation expenditure (e.g., "80.10bnđ") with YoY % change.
    *   **Total Trips:** Total volume of shipments (e.g., "46K") with YoY % change.
    *   **Average Cost per CBM:** Unit cost efficiency based on volume (e.g., "153K đ") with YoY % change.
    *   **Average Cost per KM:** Unit cost efficiency based on distance (e.g., "12.49K") with YoY % change.
*   **Cost & Operational Breakdowns:**
    *   **Cost by Payload:** Visualizes cost distribution across different vehicle payload capacities (X-axis shows payload categories like 2, 5, 15, 8, 10 – *units like 'Tons' would be clarified in a real scenario*).
    *   **Total Trips by Province:** Highlights key regions by shipment volume. The chart effectively handles and displays data for entries where province information might be "(Blank)".
    *   **Cost/CBM by Province:** Compares unit cost efficiency (e.g., "1003K") across various provinces.
    *   **Load Factor by Province (%):** Assesses average vehicle capacity utilization per province.
*   **Trend Analysis (Time Series):**
    *   **Average Load Factor (%):** Tracks the historical trend of overall load efficiency from 2020-2025.
    *   **Total Cost (Billion VND):** Illustrates the evolution of total transportation expenses from 2020-2025, including any projected figures (e.g., for 2025).
*   **Geospatial Analysis:**
    *   **Total Cost by Province (Map):** An interactive map visualizing geographic cost distribution. *Color intensity on the map (e.g., shades of red and blue) would ideally be explained by a legend in a live dashboard to indicate cost magnitude.*
*   **Interactive Elements:**
    *   Navigation pane with slicers for Year (buttons), Province (dropdown), and Payload (dropdown).
    *   A "RESET" button to clear all slicer selections for user convenience.
    *   **Custom Report Page Tooltip (for Map):** On hovering over a province (e.g., "Bình Phước" in the sample), a tooltip displays: `Province Name (Tỉnh)`, `Total Cost`, `% of Grand Total Cost (% Cost)`, and `Total Trips`.
        ```markdown
    ![Tool Tips Province](https://github.com/user-attachments/assets/41bb0acd-0cd8-46a3-bd8e-c2d21619f899)

### 2. Vendor Analysis Page: Managing Partner Performance

*This page focuses on a detailed evaluation and comparison of third-party logistics providers, crucial for effective vendor relationship management.*

![Vendor Page](https://github.com/user-attachments/assets/51a6cda8-c03e-49db-9b66-dc7b089728f8)


*   **Vendor-Specific KPIs:**
    *   **Total Cost (attributed to Vendors):** With % of grand total.
    *   **Number of Active Vendors.**
    *   **Overall Avg Cost Per Trip (Vendors).**
    *   **Average of % Load (Vendors):** Overall load factor for vendor operations, with an indicator such as "Không đạt" (Not Met) if performance is below target. *(Ideally, this overall average is a weighted calculation, not a simple average of individual vendor load factors).*
*   **Vendor Contribution & Ranking:**
    *   **Total Cost By Vendor:** Bar chart identifying top vendors by expenditure, including an "Others" category.
    *   **Total Trip By Vendor:** Bar chart ranking vendors by shipment volume, including "Others".
*   **Comparative Vendor Performance Charts:**
    *   **Avg Cost Per Trip by Vendor:** Bar chart comparing individual vendor unit costs. *Adding an overall average reference line to this chart would further enhance comparability.*
    *   **Avg Cost Per CBM by Vendor:** Similar comparison for CBM-based unit costs. *(An overall average reference line would be beneficial here too).*
*   **Detailed Vendor Performance Table:** A matrix summarizing key metrics for each listed vendor:
    *   `Vendor Name`, `% Total Cost`, `Total Trips`, `Average % Load Factor`, `Average Cost Per Trip`, `Average Cost Per CBM`.
    *   The "Total" row provides aggregated figures for the listed vendors. *Calculations for averages and percentages in the total row should reflect true overall values.*
*   **Vendor Cost Trend Over Time:** Line chart visualizing cost trends (e.g., for "Khánh Châu" and "Quang Tường") from 2022-2025, including any projected data.
*   **Interactive Elements:** Slicers for Year, Vendor Name (dropdown), and Province (dropdown); "RESET" button.
*   **Custom Report Page Tooltip (for Vendor Charts/Table):** On hovering over a vendor, a tooltip (as shown for Vendor "247" in sample screenshots) displays: `Vendor ID/Name`, `Key Performance Indicators (Average of % Load, Cost Per Trip, Cost Per CBM)`, and `Top 3 Provinces served by that vendor by Total Cost`.
    ```markdown
![Tool tips Vendor](https://github.com/user-attachments/assets/7397276a-f582-4069-81d8-09561150487b)


### 3. In-house Fleet Analysis Page: Optimizing Internal Resources

*This page is dedicated to analyzing the efficiency and productivity of the company-owned/operated fleet and its drivers.*

![Inhouse Page](https://github.com/user-attachments/assets/bbb8933e-6ccd-4a6d-92c7-4e7c4e8da2f5)


*   **In-house Fleet KPIs:**
    *   **Total Trips (In-house):** With YoY % change.
    *   **Total Distance:** Total distance covered by the in-house fleet (e.g., "632.72K" - unit like Km would be specified), with YoY % change.
    *   **Avg Trip/Driver:** Overall driver trip productivity, with YoY % change.
    *   **Total Day Active (Drivers):** Aggregate of days drivers were operational, with YoY % change.
*   **Driver & Vehicle Performance Breakdown:**
    *   **Total Trips by In-house Payload Capacity:** Shows utilization of different vehicle types within the fleet. *(X-axis "Tải trọng" means Payload Capacity).*
    *   **Top 5 Drivers by Total Distance Covered.**
    *   **Load Factor By In-house Payload Type.** *(X-axis labels like 0.90, 0.50 represent payload categories and would be defined in a real scenario).*
    *   **Top 5 Drivers by Active Days.**
    *   **Driver Performance Scatter Plot:** A key visual plotting `Total Trips` vs. `Average Trip Distance` (the X-axis label "Total Distance" in the screenshot might represent Average Trip Distance for this type of plot) for each driver. Includes average reference lines (horizontal and vertical red lines) to segment drivers into performance quadrants.
*   **Detailed Driver Performance Table:** A comprehensive table for each driver:
    *   `Driver Name (Lái xe)`, `Total Trips`, `Active Days`, `Average % Load Factor`, `Total Distance`, `Average Trips per Active Day (Daily Trip)`.
*   **Interactive Elements:** Slicers for Year, Payload Type (Trọng tải), and Driver Name (Lái xe); "RESET" button.
*   **Drill-through:** Functionality to navigate from a driver's name (in table or scatter plot) to a dedicated "Drill Through Driver Detail" page.
*   **Custom Report Page Tooltip (for Driver Scatter Plot):** On hovering over a driver, a tooltip displays a mini-profile: `Driver Name`, `Total Trip`, `Total Distance`, `Active Days`, `% Load`, `Daily Trip`.
    ```markdown
![Tool Tips Driver](https://github.com/user-attachments/assets/6184c55d-70b4-4fe3-83ac-77964d479229)


### 4. Drill Through Driver Detail Page

*This dedicated page provides an in-depth look at the performance and activity trends of a single, selected driver (e.g., "DRIVER A"), accessed via drill-through.*

![Drill Through Driver Detail](https://github.com/user-attachments/assets/53146f0b-d59f-49bd-84ab-13e28a6505da)


*   **Selected Driver's KPIs:** Prominently displays the selected `Driver Name` along with their specific `Total Trips`, `Total Distance`, `Active Days`, `Average % Load`, and `Average Trips per Driver`.
*   **Monthly Performance Trends for Selected Driver:**
    *   Combined Column & Line Chart: `Avg Trips/Driver` (columns) and `Total Distance` (line) by month.
    *   Line Chart: `Average % Load Factor` by month.
*   **Recent Trips Table:** Lists details of the driver's recent trips: `Trip Date (Ngày giao)`, `Cargo Details (Khối hàng - Cargo Volume/Weight?)`, `Vehicle Details (Khối xe - Vehicle Capacity?)`, `Distance`.
*   **Trip Characteristic Breakdown:** A Pie chart visualizing the "Average of % Load" (this could represent the distribution of the driver's trips across different Load Factor bins, e.g., 25%, 34%, 41% of trips fall into specific load categories).

---

## Technical Skills & Tools Utilized

*   **Primary Tool:** Microsoft Power BI Desktop
*   **Data Transformation (Power Query / M Language):**
    *   Connected to and integrated data from various sources (e.g., Excel files, CSVs - *specifics anonymized*).
    *   Performed comprehensive data cleaning, preprocessing, and shaping including handling missing values, standardizing data types, merging/appending queries, and creating custom/conditional columns for robust analysis.
*   **Data Modeling:**
    *   Designed and implemented a relational data model, likely a Star Schema, with a central Fact table (e.g., `Fact_Trips`) and multiple Dimension tables (`Dim_Date`, `Dim_Vendors`, `Dim_Drivers`, `Dim_Provinces`, `Dim_Payloads`).
    *   Established and managed table relationships, optimizing for query performance and data integrity.
    *   Implemented a dedicated Date dimension table for advanced time intelligence calculations.
*   **DAX (Data Analysis Expressions):**
    *   Authored a wide array of DAX measures for dynamic calculations: YoY changes, averages (per trip, per CBM, per KM, per driver, per active day), percentages (% Load Factor, % of Total), Top N rankings, and complex conditional aggregations.
    *   Leveraged key DAX functions such as `CALCULATE`, `SUMX`, `AVERAGEX`, `DIVIDE`, `FILTER`, `ALL`, `ALLEXCEPT`, `VALUES`, `DISTINCTCOUNT`, `SAMEPERIODLASTYEAR`, `IF`, `SWITCH`, `TOPN`, `RANKX`.
    *   Created Calculated Columns where necessary for categorization (e.g., Load Factor Bins, Payload Type grouping) and simplified attributes for reporting.
*   **Data Visualization & Dashboard Design:**
    *   Employed a diverse set of appropriate visuals (Column charts, Line charts including combined charts, Scatter plots, Maps, Tables, KPI Cards, Slicers) to best represent different types of data and convey insights effectively.
    *   Focused on creating an intuitive, user-friendly, and visually appealing interface with consistent branding (colors reflecting the "LOGO" theme, clear typography).
    *   Implemented advanced interactive features:
        *   **Custom Report Page Tooltips:** Designed dedicated report pages to act as rich, context-sensitive tooltips, providing granular details on hover without cluttering the main view.
        *   **Drill-through:** Enabled users to navigate seamlessly from summary views to detailed information (e.g., from a driver in a list to their individual performance page).
        *   **Slicers & Cross-filtering:** Implemented for dynamic data exploration across all visuals on a page.
        *   **"RESET" button:** Provided for user convenience to clear all active filters.
        *   **Conditional Formatting:** Applied strategically in tables and charts to visually highlight outliers, trends, or performance against benchmarks.

---

## Key Analytical Insights & Outcomes (Illustrative)

> This dashboard empowers users to:
> *   Identify cost hotspots by province or payload type, enabling targeted cost reduction efforts.
> *   Benchmark vendor efficiency on unit costs and load utilization, providing a clear basis for performance discussions and contract negotiations.
> *   Profile driver productivity based on volume, distance, active operational days, and load efficiency, facilitating fair evaluations and identifying coaching opportunities.
> *   Classify drivers into distinct performance segments using the scatter plot, allowing for tailored management strategies.
> *   Track performance trends over time to detect emerging issues, confirm the impact of improvement initiatives, or understand seasonal variations.
> *   Provide robust, data-backed evidence for strategic decisions regarding fleet management, vendor selection, and network optimization.

---

## Conclusion & Potential Future Enhancements

This Power BI Transportation Analysis dashboard serves as a powerful analytical tool, transforming complex logistics data into clear, actionable intelligence. It is designed to be a critical asset for operational monitoring, strategic planning, and fostering a culture of continuous improvement in transportation management.

**Potential future enhancements could include:**

*   **Detailed In-house Fleet Costing:** Integrating operational costs (fuel, maintenance, driver wages) for a comprehensive cost-benefit analysis against outsourcing.
*   **On-Time Delivery (OTD) Tracking & Analysis:** Incorporating OTD metrics for both vendors and the in-house fleet to measure service levels.
*   **Predictive Analytics:** Developing forecasting models for future transportation costs, demand fluctuations, or potential service disruptions.
*   **Advanced Route Optimization Analysis:** Integrating with routing data to identify more efficient delivery paths and schedules.
*   **Sustainability & Environmental Impact Metrics:** Adding KPIs related to CO2 emissions or fuel efficiency per trip/ton-km.

---

## Important Note on Data Privacy & Project Sharing

The Power BI project file (.pbix) for this dashboard is **not shared publicly** in this repository. This decision is due to the dashboard's original connection to confidential and proprietary company data.

The screenshots and descriptions provided herein showcase the dashboard's structure, design, analytical capabilities, and the technical skills employed in its development. All sensitive data within these visuals has been **anonymized, replaced with sample data, or obscured** to rigorously protect company information and ensure confidentiality.

The primary purpose of this portfolio piece is to demonstrate my proficiency in Power BI development, data modeling, DAX, and dashboard design for logistics and transportation analysis. I am enthusiastic about discussing the methodologies, technical challenges, and specific DAX solutions implemented in this project in more detail during an interview.

---

## Contact

*   **LinkedIn:** `[[Your LinkedIn Profile URL]](https://www.linkedin.com/in/charlestran105/)`
*   **Email:** `Charlestran.work@gmail.com`
*   **(Optional) Portfolio Website:** `[Your Portfolio Website URL]`
