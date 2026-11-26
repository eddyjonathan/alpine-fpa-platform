# Alpine Trail Outfitters — FP&A Data Platform

End-to-end FP&A (financial planning & analysis) platform built on Databricks,
using a synthetic company: 4 entities, 3 years of general ledger, budget,
forecasts, sales volumes and headcount.

## Architecture
CSV files → Unity Catalog Volume → COPY INTO → Bronze Delta tables
→ dbt Core (Silver / Gold) → Power BI

## Status
- [x] Bronze ingestion (COPY INTO, idempotent, DECIMAL money types, lineage columns)
- [ ] dbt staging models
- [ ] dbt P&L marts + tests
- [ ] Power BI Budget vs Actual dashboard
