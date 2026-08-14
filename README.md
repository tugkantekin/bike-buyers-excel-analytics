# bike-buyers-excel-analytics
Excel data cleaning, pivot table, and dashboard project on a 1,000-record customer dataset
Bike Buyers Customer Analytics (Excel)

An end-to-end Excel analytics project: cleaning a raw customer dataset, engineering a segmentation field, building a PivotTable, and designing a dashboard to answer a core business question — which customer profiles are most likely to purchase a bike?

Dataset
Source sheet: bike_buyers (raw data, 1,026 rows)
Working sheet: Working Sheet (1,000 cleaned rows used for analysis)
Fields: ID, Marital Status, Gender, Income, Children, Education, Occupation, Home Owner, Cars, Commute Distance, Region, Age, Purchased Bike
What I did

Data cleaning — standardized categorical values (e.g. M/S → Married/Single, M/F → Male/Female) and removed rows with inconsistent or missing entries, taking the raw set from 1,026 to 1,000 clean records.
Feature engineering — created an Age Brackets column (Adolescent / Middle Age / Old) to make purchase behavior easier to segment and compare.
PivotTable analysis — built a PivotTable showing average income by gender, cross-tabbed against purchase outcome (Yes/No).
Dashboard — assembled a one-page dashboard with three charts:
Avg Income Per Purchase
Customer Commute
Customer Age Brackets

Key findings

Segment	Purchase rate
Overall	48.1% Yes / 51.9% No
Commute 2–5 miles	58.6%
Commute 10+ miles	29.7%
Middle Age bracket	54.6%
Old bracket	31.2%
Pacific region	58.9%
Europe region	49.3%
North America region	43.3%

Takeaways:

Commute distance is one of the strongest behavioral signals — customers close to their commute hub convert far better than long-distance commuters, likely reflecting bikes as a practical transport choice rather than a leisure purchase.
Middle-aged customers are the strongest-converting age segment by a wide margin.
Regional differences are meaningful (Pacific vs. North America is a ~15-point gap), suggesting region-specific marketing could outperform a one-size-fits-all approach.

(Average income by gender/purchase-outcome is available in the PivotTable but wasn't a primary driver of purchase behavior in this dataset — worth noting as a "checked, not a strong signal" finding.)

Tools
Microsoft Excel — data cleaning, PivotTable, native chart objects
No external BI tool used; all analysis and visualization built natively in the workbook

Repo structure
├── bike_buyers_excel_project.xlsx   # Full workbook (raw data, working sheet, pivot table, dashboard)
├── images/
│   ├── dashboard.png                # Screenshot of the Dashboard tab
│   └── pivot_table.png              # Screenshot of the PivotTable tab
└── README.md

