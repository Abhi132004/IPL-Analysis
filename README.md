# IPL Analysis using Azure Databricks

## Project Description

This project aims to analyze Indian Premier League (IPL) data using Azure Databricks. The project leverages the power of Apache Spark, a fast and general-purpose cluster computing system, to analyze large datasets.

## Architecture Diagram

![IPL Data Analysis using Databricks](images/ipl_data_analysis_using_databricks.png)

The architecture diagram above depicts the flow of data in the project. The IPL data is sourced from https://cricsheet.org/downloads/. The data is then ingested into Azure Blob Storage, which serves as a data lake. Azure Databricks is used to read and process the data, and the results of the analysis are stored in Azure SQL Database.

## Getting Started

To get started with this project, follow the steps below:

1. Create an Azure Databricks workspace and start a new cluster. You can choose the lowest configuration cluster to start with, which is the Standard_DS3_v2 instance with 2 cores and 14 GB RAM.

2. Create an Azure Data Lake Storage Gen2 (ADLS Gen2) account in the Azure portal.

3. In the ADLS Gen2 account, create a container for storing the IPL data.
4. In the Azure portal, create an Azure Key Vault.

5. Add a secret to the Key Vault that contains the ADLS Gen2 storage account key. This allows the Databricks cluster to access the ADLS Gen2 container.
## Usage

Azure Databricks is used to process the IPL data. The data is read from Azure Blob Storage, and processed using Spark streaming DataFrames and delta live tables. Various analyses are performed on the data, including but not limited to:

- Top batsmen and bowlers of the tournament
- Team-wise and player-wise statistics
- Analysis of player performance in various scenarios

The results of the analysis are stored in delta tables, and are visualized using databricks visualization. Interactive dashboards are created to display the results of the analysis.

## Teaser

https://user-images.githubusercontent.com/65663124/235992291-1a7728bb-dfe7-4998-b64e-2f423fd8e417.mp4

## Sample Output
![IPL](https://user-images.githubusercontent.com/65663124/236008312-88d732c0-33fc-48f6-8b47-567b4c04af68.png)



## Contact Information
https://www.linkedin.com/in/abhishek-pokale-980883228/
https://www.linkedin.com/in/tanmay-singh-228097272/
https://www.linkedin.com/in/aryan-saklani-87706b21b/


