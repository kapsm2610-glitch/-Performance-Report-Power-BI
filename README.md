# 📊 Performance Report — Power BI

A single-page Power BI report designed to track and compare sales performance across years, products, and geographies using Year-to-Date (YTD) metrics.

---

## 📁 File Info

| Property | Details |
|---|---|
| **File** | `Performance_Report.pbix` |
| **Tool** | Microsoft Power BI Desktop |
| **Canvas Size** | 1280 × 720 px |

---

## 📐 Data Model

### Tables

| Table | Description |
|---|---|
| `_Measures` | All calculated DAX measures |
| `Dim_Date` | Date dimension with full hierarchy (Year → Quarter → Month) |
| `Dim_Account` | Customer/account dimension including country |
| `Dim_Product` | Product dimension with product type and name |
| `Slc_Values` | Supporting table for the dynamic metric slicer |

### Key DAX Measures

| Measure | Description |
|---|---|
| `S_YTD` | Sales — Year-to-Date |
| `S_PYTD` | Sales — Prior Year-to-Date |
| `YTD vs PYTD` | Variance between current and prior year sales |
| `GP%` | Gross Profit Percentage |

---

## 🧩 Visuals

| # | Visual Type | Purpose |
|---|---|---|
| 1 | **KPI Cards** | Headline metrics: S_YTD, S_PYTD, YTD vs PYTD, GP% |
| 2 | **Advanced Slicer** | Switch between metric types dynamically |
| 3 | **Year Slicer** | Filter the entire report by calendar year |
| 4 | **Treemap** | Bottom 10 countries by YTD vs PYTD variance |
| 5 | **Waterfall Chart** | Variance breakdown by Month, Country, Product Type, and Product Name |
| 6 | **Line & Stacked Column Combo** | S_YTD vs S_PYTD trend by Month/Quarter and Product Type |
| 7 | **Scatter Chart** | GP% vs S_YTD plotted by Account |
| 8 | **Title Card** | Dynamic report title |

---

## 🔍 How to Use

1. Open `Performance_Report.pbix` in Power BI Desktop or publish to Power BI Service.
2. Use the **Year Slicer** to select the reporting year.
3. Use the **Advanced Slicer** to switch between performance metrics.
4. The **KPI Cards** give an instant snapshot of headline numbers.
5. Drill into the **Waterfall Chart** to identify which months, countries, or products drive variance.
6. Use the **Scatter Chart** to spot accounts with high revenue but low margins (or vice versa).

---

## ⚙️ Requirements

- Power BI Desktop (April 2024 release or later)
- Or access via [Power BI Service](https://app.powerbi.com)

---

## 📝 Notes

- All model relationships were defined manually — no auto-created relationships.
- No Row-Level Security (RLS) is configured in this file.
