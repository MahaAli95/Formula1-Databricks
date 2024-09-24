# Formula 1 Data Pipeline with Azure Databricks
This project implements an end-to-end data engineering solution using Azure Databricks, Azure Data Factory, and Power BI to analyze Formula 1 racing data. The solution ingests data from the Ergast API, transforms it using a series of Databricks notebooks, and visualizes the results using Power BI dashboards.
Solution Architecture

    Data Ingestion:
        Data is sourced from the Ergast API and stored in the Azure Data Lake Storage (ADLS) Raw Layer.
        Azure Data Factory (ADF) orchestrates the pipeline to pull data into ADLS.

    Data Transformation:
        Transformation is done using PySpark in Databricks.
        Data flows through the Ingested Layer and is processed into the Presentation Layer using Delta Lake for optimized performance.
        Key transformations include data cleaning, schema application, and creation of delta tables.

    Data Analysis:
        Transformed data is analyzed using Databricks SQL.
        We perform aggregations and joins to derive insights like driver standings, race results, and constructor performance.

    Reporting:
        Final output is visualized in Power BI, allowing for dynamic, interactive reports and dashboards that provide insights into the Formula 1 season’s trends and performance.

Key Technologies

    Azure Data Factory: Orchestration of data workflows.
    Azure Data Lake Storage: Scalable storage for raw and transformed data.
    Azure Databricks: Processing and transformation using PySpark.
    Delta Lake: Enables efficient storage and real-time analytics.
    Power BI: Visualization and reporting.

How to Use

    Clone the repository.
    Configure your ADF pipeline and Databricks workspace with the provided notebooks.
    Ensure your API keys and storage credentials are properly set up.
    Execute the pipeline to ingest and transform the data.
    Visualize the results using Power BI templates.
