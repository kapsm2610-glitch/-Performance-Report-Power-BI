# -Performance-Report-Power-BIA single-page Power BI report designed to track and compare sales performance across years, products, and geographies using Year-to-Date (YTD) metrics.

📁 File Info
PropertyDetailsFilePerformance_Report.pbixToolMicrosoft Power BI DesktopPBI Version2.128.1039.0Report Release2024.04Created FromPower BI Cloud ServiceCanvas Size1280 × 720 px

📋 Report Pages
Performance Report (single page)
The report contains one page with a comprehensive set of visuals for analysing year-over-year sales performance.

📐 Data Model
Tables
TableDescription_MeasuresAll calculated DAX measuresDim_DateDate dimension with a full date hierarchy (Year → Quarter → Month)Dim_AccountCustomer/account dimension including countryDim_ProductProduct dimension with product type and product nameSlc_ValuesSupporting table for the dynamic metric slicer
Key Measures
MeasureDescriptionS_YTDSales — Year-to-DateS_PYTDSales — Prior Year-to-DateYTD vs PYTDVariance between current and prior year salesGP%Gross Profit Percentage_Report titleDynamic report title label

🧩 Visuals
#Visual TypeTitle / Purpose1KPI CardsDisplays headline metrics: S_YTD, S_PYTD, YTD vs PYTD, and GP%2Advanced SlicerAllows switching between metric types (Sales, GP%, etc.)3Year SlicerFilters the entire report by calendar year4TreemapBottom 10 YTD vs PYTD | Country — highlights underperforming countries5Waterfall ChartBreaks down YTD vs PYTD variance by Month, Country, Product Type, and Product Name6Line & Stacked Column ComboCompares S_YTD and S_PYTD trends by Month/Quarter, segmented by Product Type7Scatter ChartPlots GP% vs S_YTD by Account — useful for identifying high-value or at-risk accounts8Title CardDisplays the dynamic report title

🔍 How to Use

Open Performance_Report.pbix in Power BI Desktop (version 2.128+) or publish to Power BI Service.
Use the Year Slicer to select the reporting year.
Use the Advanced Slicer to switch between different performance metrics.
The KPI Cards at the top give an instant snapshot of headline numbers.
Drill into the Waterfall Chart to identify which months, countries, or products are driving the YTD vs PYTD variance.
Use the Scatter Chart to spot accounts with strong revenue but low margins (or vice versa).


⚙️ Requirements

Power BI Desktop 2.128.1039.0 or later (April 2024 release or newer)
Or access via Power BI Service (app.powerbi.com)


📝 Notes

The report was originally created from the Power BI Cloud Service.
No row-level security (RLS) roles are defined in this file.
No auto-created relationships are present — all model relationships were defined manually.
