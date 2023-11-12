# DEAssessment2-cjx

This asasignment is completed using Jupyter Notebook and data is stored locally in .csv files, following datalake design.
The answers are presented using PowerBI.

## Setup Guide
1. Download the repo to your local machine
2. Install Anaconda (If you do not have Jupyter Notebook) (https://www.anaconda.com/download/)
3. Install PowerBI Desktop
4. Launch Jupyter Notebook
5. Navigate to the directory where you saved this repo to
6. Run the ETL Scripts in sequence.


## ETL Scripts
1. 01 - Data Ingestion Script.ipynb
2. 02 - ETL to Silver Script.ipynb
3. 03 - ETL to Gold.ipynb

## Data storage
1. \Datalake

## PowerBI
1. KPI_Dashboard.pbix

### What I've done
1. I've created 3 separate scripts to represent each data movement from bronze, to silver and finally to gold layer.
2. Data are stored in \Datalake folder.
3. First ETL script makes multiple API calls to download all commits for the past 6 months and store them in \Datalake\bronze
4. Second ETL script process each file and retrieves specific data items and consolidate into a staging file, stored in \Datalake\silver
5. Third ETL script takes the staging file and output 3 distinct dataset for each query in the assignment, stored in \Datalake\gold
6. The PowerBI file takes the 3 dataset in gold layer to populate the dashboard.

