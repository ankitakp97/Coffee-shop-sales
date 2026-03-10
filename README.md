# Coffee Shop Sales

A compact analytics project for exploring coffee shop performance and turning transaction data into practical business decisions.

## Overview
This repository is intended as a clean foundation for sales analysis, with emphasis on:
- consistent KPI definitions,
- reproducible transformations,
- and presentation-ready outputs for stakeholders.

## Business Questions
- Which products and categories contribute most to revenue?
- When are demand peaks by hour and day of week?
- How do order volume and average order value move over time?
- Which items are high-volume but low-margin candidates for optimization?

## KPI Definitions
| KPI | Definition |
|---|---|
| Total Revenue | Sum of `unit_price × quantity` |
| Total Orders | Count of distinct order IDs |
| Units Sold | Sum of item quantities |
| Average Order Value (AOV) | `Total Revenue ÷ Total Orders` |
| Revenue by Category | Revenue grouped by product category |
| Peak Hours | Hourly buckets ranked by order count or revenue |

## Suggested Repository Layout
```
Coffee-shop-sales/
├── data/
│   ├── raw/           # source extracts
│   └── processed/     # cleaned modeling-ready tables
├── sql/               # KPI and reporting queries
├── notebooks/         # exploratory analysis
├── dashboards/        # BI files / app configs
├── reports/           # insight summaries
└── README.md
```

## Getting Started
1. Place source files in `data/raw/`.
2. Create cleaned datasets in `data/processed/` (typed columns, null handling, deduplication).
3. Build KPI queries in `sql/` and validate totals against source data.
4. Publish visuals (dashboard or notebook report) focused on decisions, not just charts.

## Quality Checklist
- Use one canonical definition per KPI.
- Keep date/time logic explicit (timezone, week start, holiday handling).
- Separate transformation logic from presentation logic.
- Document assumptions in report footnotes.

## Contributing
PRs that improve data quality, metric reliability, query performance, or dashboard clarity are welcome.

## License
Add a license file (for example, MIT) if you plan to distribute this project.
