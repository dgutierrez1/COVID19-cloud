# COVID19-cloud

This gist will describe the process to:
1. Do a ETL process from GCP COVID public data into Azure BlobStorage
2. Execute SQL queries from Databricks
3. 

# ETL to Azure Blob Storage
The COVID 19 open data initially is located in Big Query. Although Big Query is not an storage query it is the only way access the data.
To make the data available from external services like Blob Storage the COVID table needs to be **copied to a project you own**. That will be the first step.

Open the `covid19_open_data` table and select `Copy Table`

![alt text](./imgs/copy-table.png)

Then select the project, dataset and table you want to copy it into
![alt text](./imgs/copy-table1.png)