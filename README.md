End-to-End Azure Data Engineering
This repository contains the project "End-to-End Azure Data Engineering", which demonstrates a comprehensive solution using Azure for data engineering, starting from a local SQL database and culminating in Power BI reporting.

🙏 Special Thanks:

Inspired by Mr. K Talks Tech.
🎯 Business Objective
Learning Opportunity: Focus on common data engineering practices, especially ETL pipeline techniques.
Target Audience: Beneficial for small to medium-sized businesses looking to migrate their local data to the cloud.
🌐 Current Environment
Data Source: AdventureWorks dataset from Microsoft.
Setup:
On-premises Microsoft SQL server on a personal computer.
Dataset imported using Microsoft SQL Server Management Studio.
New user profile "nik" created.
"nik" profile’s password saved as a Secret in Azure Key Vault.
🚀 Implementation Steps
1️⃣ Data Ingestion
Tool: Azure Data Factory.
Process:
Install Self-Hosted Integration Runtime.
Connect Azure Data Factory with local SQL Server.
Set up a copy pipeline to Azure Data Lake's "bronze" folder.
2️⃣ Data Transformation
Tool: Azure Databricks using PySpark.
Process:
Transition data through "bronze" to "silver" and "gold" layers.
Use Databricks notebooks for transformation.
Automatically update Azure Data Factory for notebook execution.
3️⃣ Data Loading
Tool: Azure Synapse.
Process:
Link Azure Storage (Gold Folder) to Azure Synapse.
Extract table information as SQL view.
Store views in server-less SQL Database.
4️⃣ Data Reporting
Tool: Microsoft Power BI.
Process:
Connect to the cloud pipeline using DirectQuery.
Develop a report visualizing the AdventureWorks dataset.
5️⃣ Final Pipeline Test
Validation: Add new customers to SQL database and observe updates in Power BI report.
🧐 Conclusion and Limitations
Project Scope: Demonstrates the ability to create an ETL cloud solution with Azure.
Considerations:
Small dataset to minimize compute and storage costs.
Use of multiple applications for a simple task.
Project could have been simplified but expanded for learning.
🛠 About
Scope: End-to-End Azure Data Engineering Pipeline for ETL and Analytics Reporting on AdventureWorks2022LT Database.
📚 Topics
#azure #python3 #azure-storage #powerbi #t-sql #ssms #azuredatafactory #pyspark-notebook #azuredatabricks #azuresynapse #azure-data-lake-gen2
🌟 Stars
🌟 0 stars
👀 1 watching
🍴 1 fork
