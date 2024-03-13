# End-to-End Azure Data Engineering Pipeline

## 🌟 Introduction
This project demonstrates an automated end-to-end Azure data engineering solution, beginning with a local SQL database and culminating in Power BI reporting.

Special thanks to Mr. K Talks Tech for the inspiration behind this project.

## 🎯 Business Objective
- To provide a hands-on experience in common data engineering practices, focusing on ETL pipeline techniques.
- To showcase skills critical for small to medium-sized businesses planning to migrate their data to the cloud.

## 🏭 Current Environment
- Utilized the AdventureWorks dataset from Microsoft.
- Set up an on-premises Microsoft SQL server.
- Imported the dataset using Microsoft SQL Server Management Studio.
- Stored credentials in Azure Key Vault.

## ⚙️ Implementation Steps

### 1️⃣ Data Ingestion
- **Tools**: Azure Data Factory
- **Process**:
  - Installed Self-Hosted Integration Runtime.
  - Established connection between Azure Data Factory and local SQL Server.
  - Set up a pipeline to transfer tables to Azure Data Lake's "bronze" folder.

### 2️⃣ Data Transformation
- **Tools**: Azure Databricks (PySpark)
- **Process**:
  - Transformed data from "bronze" to "silver" and "silver" to "gold" using Databricks notebooks.
  - Updated Azure Data Factory to automate these transformations.

### 3️⃣ Data Loading
- **Tools**: Azure Synapse
- **Process**:
  - Created links from Azure Storage (Gold Folder) to Azure Synapse.
  - Wrote procedures for SQL view extraction.
  - Stored views within Synapse's server-less SQL Database.

### 4️⃣ Data Reporting
- **Tools**: Power BI
- **Process**:
  - Connected Power BI directly to the cloud pipeline using DirectQuery.
  - Developed a Power BI report for visualizing dataset data.

### 5️⃣ Pipeline Testing
- **Verification**: Added new entries to the SQL database to ensure dynamic updates in the Power BI report.

## 🚀 Conclusion and Limitations
- This project illustrates the creation of an ETL cloud solution using Azure.
- Some points to consider:
  - Small dataset used to minimize costs.
  - Multiple applications were used for learning purposes.
  - The project's complexity is scalable based on dataset size and processing needs.

## 💡 About
This project is an end-to-end demonstration of an Azure Data Engineering Pipeline, involving ETL processes and analytics reporting on the AdventureWorks2022LT Database.

## 📚 Topics
`azure` `python3` `azure-storage` `powerbi` `t-sql` `ssms` `transact-sql` `azure-data-factory` `pyspark-notebook` `azure-databricks` `azure-synapse-analytics` `azuredatalakegen2` `azure-synapse-serverless-sql` `microsoft-entra`

## ⭐ Stars
![Stars](https://img.shields.io/github/stars/your-username/your-repo?style=social)

## 🛠️ Resources
- [AdventureWorks2022LT Sales Database](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)
- [Mr. K Talks Tech video on E2E Azure Data Engineering Project](https://www.youtube.com/watch?v=iQ41WqhHglk&t=3624s)

## ©️ License
GPL-3.0

---

© 2024 GitHub, Inc. Terms Privacy Security Status Docs
