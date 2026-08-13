# Laptop Manufacturing Operations Analytics

A comprehensive Excel-based analysis of 6,000 manufacturing records spanning production, profitability, quality, inventory, warranty, maintenance, logistics, and capacity planning. Investigates 8 critical business questions and delivers data-backed recommendations for cost control, quality improvement, and operational efficiency.

## Key Findings

**Production & Profitability Paradox:**
- Q2 shows 20% production growth, but operating profit **declined 14%** — indicating rising production costs outpacing revenue growth
- Root cause: material costs and supplier inefficiencies

**Inventory Crisis:**
- Q4 unsold inventory spike to 4,248 units — a major cash flow risk
- Regions: North and South show disproportionate excess stock

**Quality Variance:**
- Supplier A and Material Grade 1 show significantly lower defect rates than Supplier B (11% vs. 28%)
- Recommendation: audit Supplier B's QA processes or reduce order volume

**Maintenance & Downtime:**
- Machine line 3 and Shift C experience 35% higher downtime than average
- Cost impact: ~₹2.1M in lost production hours per quarter

## Analysis Methodology

**Formulas & Techniques:**
- `SUMIFS` / `COUNTIFS` / `AVERAGEIFS` for multi-dimensional aggregation (by region, supplier, material, machine, shift)
- Weighted KPI calculations: `margin = (revenue - operating_cost) / revenue`
- Pivot tables for drill-down analysis (factory, production line, supplier, material grade, machine, shift, region level)
- Conditional formatting for variance detection (red-flag thresholds)

**Data Validation:**
- 6,000 records × 65 columns processed
- Zero missing critical values
- Outlier detection via quartile analysis

## Deliverables

| Analysis | Key Metrics | Business Impact |
|----------|------------|-----------------|
| **Profitability** | Revenue, Operating Cost, Operating Profit, Margin % | Identify cost control opportunities |
| **Production** | Units Produced, Production Efficiency %, Capacity Utilization | Optimize production scheduling |
| **Quality** | Defect Rate %, Warranty Cost, Rework Rate | Improve supplier QA and material selection |
| **Inventory** | Stock Levels, Days Inventory Outstanding, Stockout Risk | Reduce cash tied up in inventory |
| **Logistics** | On-Time Delivery %, Lead Time, Shipment Cost | Streamline distribution network |
| **Maintenance** | Equipment Downtime %, Mean Time Between Failures | Reduce unplanned maintenance costs |

## Skills Demonstrated

- **Microsoft Excel** — advanced formulas, pivot tables, multi-sheet data modeling
- **Data Analysis** — drill-down investigation, variance analysis, root-cause diagnosis
- **Business Analysis** — cost-benefit reasoning, supplier/material/machine performance benchmarking
- **KPI Design** — weighted metrics, threshold-based alerting, executive summary dashboards
- **Data Visualization** — charts, conditional formatting, executive-ready reports

## How to Use This Workbook

1. **Open** `Laptop_Manufacturing_Operations_Analytics.xlsx` in Microsoft Excel
2. **Navigate** the sheet tabs for different analyses (Profitability, Quality, Inventory, etc.)
3. **Filter** by region, supplier, material, or time period using the Slicer controls (if present) or pivot tables
4. **Drill down** into specific product lines or machines to investigate anomalies
5. **Export** findings to PowerPoint or PDF for stakeholder review

## Sheets Overview

- **Summary**: Executive overview with key KPIs and exception alerts
- **Profitability**: Revenue, cost, margin analysis by region, product, and supplier
- **Production**: Units produced, efficiency %, capacity utilization trends
- **Quality**: Defect rates, warranty costs, rework analysis by supplier and material grade
- **Inventory**: Stock levels, Days Inventory Outstanding, excess stock alerts
- **Logistics**: On-time delivery %, lead times, cost per shipment
- **Maintenance**: Equipment downtime %, MTBF by machine and shift
- **Recommendations**: Data-backed action items for each business area

## Data Source

- 6,000 manufacturing records from operational database
- Period: Last 4 quarters (baseline + 3 quarters forward)
- Grain: One row per production batch (includes region, factory, product line, supplier, material, machine, shift, date)

---
