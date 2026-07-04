# food_chain_project

The Food Chain Project is an end-to-end data engineering pipeline built on Databricks Lakehouse, designed to process raw operational data from a food-supply/retail business (customers, products, pricing, and orders) into clean, analytics-ready tables.

The project follows the Medallion Architecture (Bronze → Silver → Gold), is version-controlled on GitHub, deployed through a Dev → Prod CI/CD process using Databricks Asset Bundles (DABs), and runs as a fully automated, incrementally-loading job that can be scheduled daily or weekly.

The pipeline currently orchestrates four dependent tasks — customer, product, and price dimension processing, followed by an incremental fact table load for orders — as shown in the Databricks Job Run graph below.

