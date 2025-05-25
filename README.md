# Azure Data Factory Portfolio Project – Paypal ETL Pipeline

This project showcases a real-world ETL solution built using **Azure Data Factory (ADF)**. The pipeline integrates and transforms PayPal data for analytics using ADF Data Flows, Datasets, and Pipelines.

##  Project Overview

- **Use Case**: Transform PayPal transaction and product data for analytics.
- **Technologies**: Azure Data Factory, Data Flows, Azure Blob Storage.
- **Data Flow**: Cleans, joins, and filters PayPal data.
- **Pipeline**: Orchestrates the Data Flow execution.
- **Datasets**: Source and sink definitions for external data stores.

## 🔄Data Flow: `PaypalTransformation`

This data flow performs:
- **Source Ingestion**: Imports data from `PaypalTransactions` and `PaypalProducts`.
- **Join**: Left outer join on transaction and product data.
- **Filtering**: Removes records based on `Status`.
- **Sink**: Outputs a refined dataset with 22 columns.

File: `dataflow/PaypalTransformation.json`

##  Folder Structure

azure-data-factory-portfolio/
│
├── dataflow/ # ADF data flow definitions
├── dataset/ # Source/sink datasets
├── pipeline/ # Pipeline to orchestrate data flow
├── ARMTemplateForFactory.json
├── ARMTemplateParametersForFactory.json
└── README.md
