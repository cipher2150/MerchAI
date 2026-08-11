# MerchAI

**MerchAI** is a retail data engineering project built on **Databricks** using the **Medallion Architecture**. It transforms raw retail data into clean, validated, and business-ready datasets through a structured **Bronze → Silver → Gold** pipeline.

The project uses **PySpark, Delta Lake, and SQL** to perform data ingestion, transformation, cleaning, and aggregation, creating a reliable foundation for downstream analytics and business intelligence.

---

## Architecture

```text
                    ┌─────────────────────┐
                    │    Raw Retail Data  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   🥉 Bronze Layer   │
                    │                     │
                    │  Raw Data Ingestion │
                    │  Minimal Processing │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   🥈 Silver Layer   │
                    │                     │
                    │  Data Cleaning      │
                    │  Transformation     │
                    │  Validation         │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    🥇 Gold Layer    │
                    │                     │
                    │  Business-Ready    │
                    │  Analytical Data   │
                    └─────────────────────┘

<img width="1931" height="958" alt="Screenshot 2026-08-11 at 11 51 12 PM" src="https://github.com/user-attachments/assets/5a20fdb9-2934-4580-bdaf-d30ec13961f7" />
