# **👨🏻‍💻 Walmart Sales & Retail Operations \| End-to-End Data Analytics Project**

This project represents a complete, industry-standard retail analytics workflow designed to track business performance, customer trends, and logistics fulfillment. The project leverages **Microsoft Excel** for data cleaning and preparation, and **Power BI Desktop** for building an interactive, button-navigated executive dashboard.

## **🎯 Business Problem Statement**

A retail organization wants to understand its transactional sales data, customer purchasing patterns, and logistics efficiency to maximize profitability, optimize supply chain fulfillment, and improve customer retention. Management requires data-driven clarity on how factors such as product categories, regional demographics, discount distributions, and shipping durations impact top-line revenue and bottom-line net profit.

### **❓ Overarching Business Question:**

*"How can the company leverage transactional, geographical, and operational sales data to identify profit leakages, optimize fulfillment times, and drive data-driven retail strategies?"*

## **📌 Project Deliverables**

* **Data Preparation & Cleaning (Excel):** Cleaned and structured raw transactional logs, standardizing geographic hierarchies, dates, and operational metrics.  
* **Interactive Dashboarding (Power BI):** Built a dynamic multi-page executive dashboard featuring custom button navigation, DAX metrics, KPI cards, and cross-filtering.  
* **Operational Analytics & Logistics Tracking:** Quantified supply chain efficiency by evaluating fulfillment windows (Delivery\_Days) and profit margins across regions.  
* **Strategic Reporting & Recommendations:** Synthesized analytical findings and margin outlier metrics into actionable business recommendations for executive stakeholders.  
* **GitHub Documentation:** Maintained a fully structured portfolio repository containing cleaned datasets, .pbix report files, and comprehensive Markdown documentation.

## **🏗️ Technical Architecture & Workflow**

<pre><code>
┌─────────────────────────┐      ┌─────────────────────────┐      ┌─────────────────────────┐
│     Raw Data Source     │ ───► │      Data Cleaning      │ ───► │  Business BI & Visuals  │
│      (3,203 rows)       │      │    (Microsoft Excel)    │      │   (Power BI Desktop)    │
└─────────────────────────┘      └─────────────────────────┘      └─────────────────────────┘
</code></pre>

## **📊 Dataset Summary**

* **Total Records:** 3,203 granular transaction records  
* **Attributes:** 17 comprehensive demographic, geographic, financial, and operational features  
* **Key Features:**  
  * **Identifiers & Geography:** Order\_ID, EmailID, Country, State\_Name, City  
  * **Product Details:** Category, Product\_Name  
  * **Financial & Quantity Metrics:** Sales, Quantity, Profit  
  * **Engineered Operational Metrics:** Delivery\_Days, Profit\_margin, Order\_Size, Year\_col, Month\_col

## **🛠️ Tech Stack & Tools Used**

* **Data Cleaning & Preparation:** Microsoft Excel (walmart\_cleaned\_data.xlsx)  
* **Data Visualization & Dashboarding:** Power BI Desktop (walmart\_sales\_dashboard.pbix) featuring DAX, interactive blank buttons, slicers, KPI cards, and cross-filtering  
* **Documentation & Version Control:** Git, GitHub, Markdown

## **🔍 Key Project Stages & Highlights**

### **1\. Data Preparation & Structuring (Excel)**

* **Data Normalization:** Cleaned structural data types, standardized date formats (Order\_Date, Ship\_Date), and verified text hierarchies across geographic columns (State\_Name, City).  
* **Feature Engineering:**  
  * **Delivery\_Days**: Calculated precise fulfillment duration as the day difference between shipping and order dates (mean: \~3.93 days, range: 0 to 7 days).  
  * **Profit\_margin**: Derived percentage return relative to sales via formula calculations (mean: \~21.95%, spanning positive returns down to negative margin outliers at \-210.00%).  
  * **Order\_Size**: Categorized transactions into volume-based segments.  
  * **Temporal Attributes**: Extracted Year\_col and Month\_col to empower time-series slicers and matrix aggregations.

### **2\. Business Intelligence Decisions & Key Findings**

* **Revenue Scale & Profitability Health:**  
  * Transaction sales average **\$226.49**, displaying wide variability up to a maximum of **\$13,999.96**.  
  * The aggregate portfolio maintains a solid average profit margin of **21.95%** and an average order profit of **\$33.85**.  
  * Deep-dive audit identified negative profit outliers (reaching **\-210.00%** margin), exposing specific product sub-categories impacted by heavy discounting and margin erosion.  
* **Supply Chain & Fulfillment Efficiency:**  
  * Order processing clusters efficiently around an average fulfillment duration of **3.93 days**, ranging smoothly from same-day dispatch up to a maximum window of **7 days**.

### **3\. Dashboard & Visual Insights (Power BI)**

Built a dynamic, multi-page executive dashboard featuring advanced UI elements:

* **Custom Button Navigation System:** Implemented interactive blank buttons configured with dynamic text fields, custom padding, and precise formatting states (**On hover**, **On press**, and **Default**) to enable seamless page transitions without canvas clutter.  
* **Executive KPIs:** Total Sales, Total Profit, Average Profit Margin, and Total Quantity Sold.  
* **Visual Breakdown:** Category comparison matrices, regional state-level performance filters, and fulfillment timeline trackers.

## **💡 Strategic Business Recommendations**

* **Margin & Discount Audit:** Address severe negative profit outliers (down to \-210% margin) by establishing strict discounting thresholds for vulnerable product sub-categories.  
* **Supply Chain SLA Enforcement:** Investigate tail-end 7-day delivery outliers to ensure consistent fulfillment SLA compliance across regional distribution centers.  
* **Regional Resource Allocation:** Leverage state and city-level slicers on the regional performance page to redirect focus and resources toward high-margin geographic markets.  
* **Interactive UX Standardization:** Utilize custom button navigation patterns across all report pages to ensure a clean, intuitive user experience for executive stakeholders.
