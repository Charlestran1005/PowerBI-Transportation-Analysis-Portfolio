# Power BI Transportation & Logistics Analysis - Portfolio Showcase

## Project Introduction

This project showcases a comprehensive Power BI dashboard designed to provide in-depth analysis and actionable insights into transportation and logistics operations. The primary goal was to empower stakeholders with a clear understanding of cost structures, vendor efficiencies, and in-house fleet performance, ultimately facilitating data-driven strategies for optimization and cost reduction within a dynamic supply chain environment.

The dashboard moves beyond simple reporting, offering interactive visualizations and drill-through capabilities to explore the nuances of transportation data, identify key trends, and pinpoint areas for operational improvement.

---

## Key Dashboard Objectives & Business Value

The development of this dashboard was driven by the need to address several key business questions and objectives:

*   **Cost Visibility & Control:** To gain a transparent view of total transportation expenditures, breaking them down by various dimensions such as time periods, geographical regions, payload capacities, and service providers.
*   **Vendor Performance Management:** To rigorously evaluate and benchmark the performance of external transportation vendors based on cost-effectiveness (e.g., cost per trip, cost per CBM/KM) and operational efficiency (e.g., load factor).
*   **In-house Fleet Optimization:** To analyze the productivity and efficiency of the internal fleet, with a specific focus on driver performance metrics (trips, distance, active days, load utilization) and vehicle usage patterns.
*   **Identification of Inefficiencies & Opportunities:** To proactively identify high-cost routes, underperforming vendors or drivers, and opportunities for improving load consolidation, route planning, or vehicle allocation.
*   **Strategic Decision Support:** To provide a robust analytical foundation for strategic decisions related to vendor negotiation, fleet management, network design, and overall logistics strategy.

---

##  Dashboard Structure & Core Features

The dashboard is organized into several key pages, each designed to address specific analytical needs. All pages are highly interactive, featuring dynamic filtering and custom tooltips for enhanced data exploration.

### 1. Overview Page: Holistic Performance Snapshot

*This page provides a high-level summary of the entire transportation operation.*

![Overview Page](images/overview_page_anonymized.png) 
*(Ensure this image is fully anonymized)*

*   **Key Performance Indicators (KPIs):**
    *   **Total Transportation Cost:** Overall expenditure with YoY % change.
    *   **Total Trips:** Total volume of shipments with YoY % change.
    *   **Average Cost per CBM:** Unit cost efficiency based on volume, with YoY % change.
    *   **Average Cost per KM:** Unit cost efficiency based on distance, with YoY % change.
*   **Cost Breakdown Analysis:**
    *   **Cost by Payload Capacity:** Visualizes cost distribution across different vehicle/shipment sizes.
    *   **Total Cost by Province:** Geographic cost distribution using an interactive map and a supporting bar chart for precise comparison.
*   **Operational Activity Insights:**
    *   **Total Trips by Province:** Highlights key regions by shipment volume.
    *   **Average Load Factor (%) by Province:** Assesses an_US" style="text-transform: none">verage vehicle capacity utilization per province.
*   **Trend Monitoring:**
    *   **Average Load Factor (%) Over Time:** Tracks the historical trend of overall load efficiency.
    *   **Total Cost Over Time:** Illustrates the evolution of total transportation expenses, highlighting seasonalities or significant shifts.
*   **Interactive Elements:** Slicers for Year, Province, and Payload; "Reset Filters" button; Custom report page tooltips for map and charts providing granular details on hover.

### 2. Vendor Analysis Page: Managing Partner Performance

*This page focuses on evaluating and comparing the performance of third-party logistics providers.*

![Vendor Page](images/vendor_analysis_anonymized.png)
*(Ensure this image is fully anonymized)*

*   **Vendor-Specific KPIs:**
    *   **Total Cost (Vendors):** Aggregated cost attributed to external vendors.
    *   **Number of Active Vendors:** Count of unique vendors utilized.
    *   **Overall Average Cost Per Trip (Vendors):** Fleet-wide average for outsourced trips.
    *   **Overall Average Load Factor (Vendors):** Aggregated load efficiency for vendors.
*   **Vendor Contribution & Ranking:**
    *   **Total Cost By Vendor:** Identifies top vendors by expenditure (Top N + "Others" category).
    *   **Total Trips By Vendor:** Ranks vendors by shipment volume (Top N + "Others").
*   **Comparative Vendor Performance:**
    *   **Average Cost Per Trip by Vendor:** Bar chart comparing individual vendor unit costs against the overall vendor average (via reference line).
    *   **Average Cost Per CBM by Vendor:** Similar comparison for CBM-based unit costs.
*   **Detailed Vendor Performance Table:** A matrix summarizing key metrics for each vendor, including:
    *   `% of Total Cost`, `Total Trips`, `Average % Load Factor`, `Average Cost Per Trip`, `Average Cost Per CBM`.
    *   *Conditional formatting applied to highlight high/low performers.*
*   **Vendor Cost Trend Analysis:** Line chart visualizing the cost trends over time for selected key vendors.
*   **Interactive Elements:** Slicers for Year, Vendor Name, and Province; Custom report page tooltips for detailed vendor profiles on hover (e.g., top provinces served, key KPIs).

### 3. In-house Fleet Analysis Page: Optimizing Internal Resources

*This page is dedicated to analyzing the efficiency and productivity of the company-owned/operated fleet and drivers.*

![Inhouse Page](images/inhouse_driver_performance_anonymized.png)
*(Ensure this image is fully anonymized)*

*   **In-house Fleet KPIs:**
    *   **Total In-house Trips:** Volume of trips handled internally.
    *   **Total In-house Distance:** Total kilometers covered by the in-house fleet.
    *   **Average Trips per Driver:** Overall driver productivity.
    *   **Total Driver Active Days:** Aggregate of days drivers were operational.
*   **Driver & Vehicle Performance Breakdown:**
    *   **Total Trips by In-house Payload Capacity:** Shows utilization of different vehicle types within the fleet.
    *   **Top 5 Drivers by Total Distance Covered.**
    *   **Load Factor by In-house Payload Type.**
    *   **Top 5 Drivers by Active Days.**
    *   **Driver Performance Scatter Plot:** A key visual plotting `Total Trips` vs. `Average Trip Distance` for each driver, with quadrant lines based on fleet averages. This helps segment drivers into performance categories (e.g., high volume/short-haul, low volume/long-haul, high performers, areas for attention). *Tooltip for this chart shows a mini-profile for each driver.*
*   **Detailed Driver Performance Table:** A comprehensive table for each driver, including:
    *   `Driver Name`, `Total Trips`, `Active Days`, `Average % Load Factor`, `Total Distance`, `Average Trips per Active Day (Daily Trip)`.
    *   *Conditional formatting used to highlight performance variations.*
*   **Interactive Elements:** Slicers for Year, Payload Type (Trọng tải), and Driver Name (Lái xe); "Reset Filters" button; Drill-through functionality from driver names (in table or scatter plot) to a dedicated "Driver Detail" page.

### 4. Driver Detail Page (Drill-Through)

*This page provides a deep dive into the performance and activity of a single, selected driver.*

![Driver Detail Page](images/driver_detail_anonymized.png)
*(Ensure this image is fully anonymized)*

*   **Selected Driver's KPIs:** Displays all key metrics for the specific driver (Total Trips, Total Distance, Active Days, Avg. % Load, Avg. Trip Distance, Avg. Trips per Active Day).
*   **Monthly Performance Trends for Selected Driver:**
    *   Combined Column & Line Chart: `Average Trips/Driver` (columns) and `Total Distance` (line) by month.
    *   Line Chart: `Average % Load Factor` by month.
*   **Recent/Notable Trips Table:** Lists details of the driver's last 5 trips (or top/bottom trips by a specific metric like Load Factor), including `Date`, `Origin`, `Destination`, `Vehicle Used`, `Distance`, `Actual Load`, `% Load Factor`.
*   **(Optional) Trip Characteristic Breakdown:** A Pie or Bar chart showing the distribution of the driver's trips by distance categories (e.g., Short <50km, Medium 50-150km, Long >150km) or by Load Factor bins (e.g., <70%, 70-85%, >85%).

---

##  Technical Implementation & Skills Demonstrated

This dashboard was developed using Microsoft Power BI Desktop, leveraging a range of its capabilities:

*   **Data Ingestion & Transformation (Power Query / M Language):**
    *   Connected to and integrated data from diverse sources (e.g., Excel spreadsheets, CSV files, potentially SQL databases – *describe generically*).
    *   Performed extensive data cleaning and preprocessing steps: handling missing values, correcting data types, standardizing text formats, removing duplicates.
    *   Applied transformations such as unpivoting, merging queries, appending queries, and creating conditional columns to shape the data for optimal analysis.
*   **Data Modeling:**
    *   Designed and implemented a relational data model, likely a Star Schema, with a central Fact table (e.g., `Fact_Trips`) and multiple Dimension tables (e.g., `Dim_Date`, `Dim_Vendors`, `Dim_Drivers`, `Dim_Provinces`, `Dim_Payloads`).
    *   Established and managed relationships between tables, ensuring data integrity and efficient query performance.
    *   Created a dedicated Date dimension table with a comprehensive set of date-related attributes for time intelligence.
    ```markdown
    ![Data Model Diagram (Anonymized)](images/data_model_anonymized.png) 
    ```
    *(Include your simplified, anonymized data model diagram here)*
*   **DAX (Data Analysis Expressions):**
    *   Authored numerous complex DAX measures to calculate dynamic KPIs and enable advanced analytics. Examples include:
        *   Time intelligence functions (`SAMEPERIODLASTYEAR`, `DATESYTD`, `TOTALYTD`) for YoY calculations and period-to-date aggregations.
        *   Iterator functions (`SUMX`, `AVERAGEX`, `MAXX`) for row-level calculations aggregated correctly.
        *   Context modification functions (`CALCULATE`, `FILTER`, `ALL`, `ALLEXCEPT`, `KEEPFILTERS`) for sophisticated filtering and scenario analysis.
        *   Logical functions (`IF`, `SWITCH`) for conditional calculations and categorization.
        *   Ranking and Top N functions (`RANKX`, `TOPN`) for identifying top performers or contributors.
        *   Measures for calculating averages, percentages, ratios (e.g., `DIVIDE` for safe division).
    *   Created Calculated Columns for attributes not present in the source data (e.g., grouping % Load Factor into bins).
*   **Data Visualization & Dashboard Design:**
    *   Selected a variety of appropriate visuals (Column charts, Line charts, Scatter plots, Maps, Tables, KPI Cards, Slicers) to best represent different types of data and insights.
    *   Focused on creating a clean, intuitive, and aesthetically pleasing user interface (UI) and user experience (UX).
    *   Implemented a consistent color scheme and branding elements.
    *   Utilized advanced visualization features:
        *   **Custom Report Page Tooltips:** Designed dedicated report pages to act as rich tooltips, providing contextual details on hover.
        *   **Drill-through:** Enabled users to navigate from summary views to detailed information (e.g., from a driver in a list to their individual performance page).
        *   **Bookmarks (if used):** Created bookmarks for pre-defined views or analytical scenarios.
        *   **Conditional Formatting:** Applied to tables and charts to visually highlight outliers, trends, or performance against targets (e.g., using data bars, color scales, icons).
*   **Report Interactivity:**
    *   Implemented slicers for dynamic filtering by Year, Province, Vendor, Driver, and Payload Type.
    *   Ensured cross-filtering between visuals for an integrated analytical experience.
    *   Added a "Reset Filters" button for user convenience.

---

##  Key Analytical Insights & Outcomes (Illustrative)

*Through this dashboard, stakeholders can gain insights such as:*

*   **Cost Hotspots:** Clear identification of provinces or payload types that contribute disproportionately to total transportation costs, enabling targeted cost-saving initiatives.
*   **Vendor Performance Segmentation:** Differentiation between high-performing, cost-effective vendors and those requiring performance improvement discussions or contract renegotiation, based on metrics like average cost per trip/CBM and load factor.
*   **Driver Productivity Profiling:** Understanding the varying operational styles and efficiencies of in-house drivers (e.g., high-volume short-haul specialists vs. long-haul experts vs. underutilized drivers), facilitating better work allocation and targeted training.
*   **Load Optimization Opportunities:** Pinpointing instances or patterns of low load factors (either by vendor, driver, or route) to improve freight consolidation and reduce empty miles.
*   **Trend Impact Analysis:** Assessing the impact of external factors (e.g., fuel price changes, seasonal demand) or internal initiatives on key transportation KPIs over time.
*   **Data-Backed Negotiations:** Providing concrete data to support negotiations with vendors or to justify investments in the in-house fleet.

---

## Conclusion & Potential Future Enhancements

This Power BI Transportation Analysis dashboard serves as a robust analytical tool, transforming raw transportation data into actionable intelligence. It empowers users to monitor performance, identify inefficiencies, and make informed decisions to optimize their logistics network.

**Potential future enhancements could include:**

*   **Cost Allocation for In-house Fleet:** Integrating detailed operational costs (fuel, maintenance, labor) for the in-house fleet to enable a true "apples-to-apples" cost comparison with external vendors.
*   **Route Optimization Analysis:** Incorporating route-specific data to identify opportunities for more efficient routing.
*   **Predictive Analytics:** Developing models to forecast future transportation costs, demand, or potential delays.
*   **Real-time Tracking Integration (if applicable):** Linking with telematics data for live monitoring of fleet movements and performance.
*   **Sustainability Metrics:** Adding KPIs related to CO2 emissions or fuel efficiency.

---

## <a name="data-privacy"></a>Important Note on Data Privacy & Project Sharing

The Power BI project file (.pbix) for this dashboard is **not shared publicly** in this repository. This decision is due to the dashboard's original connection to confidential and proprietary company data.

The screenshots and descriptions provided herein showcase the dashboard's structure, design, analytical capabilities, and the technical skills employed in its development. All sensitive data within these visuals has been **anonymized, replaced with sample data, or obscured** to rigorously protect company information and ensure confidentiality.

The primary purpose of this portfolio piece is to demonstrate my proficiency in:
*   End-to-end Power BI dashboard development.
*   Complex data modeling and DAX measure creation.
*   Effective data visualization and interactive report design.
*   Applying analytical thinking to solve business problems in the logistics and transportation domain.

I am enthusiastic about discussing the methodologies, technical challenges, and specific DAX solutions implemented in this project in more detail during an interview.

---

## 📞 Contact

*   **LinkedIn:** [Your LinkedIn Profile URL]
*   **Email:** [Your Email Address]
*   **(Optional) Portfolio Website:** [Your Portfolio Website URL]
