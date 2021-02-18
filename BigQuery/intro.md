#### Introduction
BigQuery is a petabyte-scale fully managed **data warehouse**
1. it's serverless
focus on the sql without worrying about the infrastructure
2. flexible pricing model 
the data stored and the bytes of data that are processing
3. data encryption and security

    You can specify the geographic locality of your data;

    Controlling access to your data can granular as specific columns;

    Work with IAM to set roles and permissions at project level;

4. geospatial data types and functions
5. foundation for BI and AI

#### Architecture Example
![Exampe](arch.jpg)

#### BigQuery: Fast SQL Engine
1. BigQuery contains two things: 
   * Fast SQL Query Engine 
   * Managed storage for datasets
2. How does BigQuery work?

   BigQuery Storage Service <-(by high speed network)-> BigQuery Query Service

   > The high speed could separate the compute and storage

   Project -> Dataset -> Tables
   >The tables are highly compressed and store in the google colossus for durability and global availability

   The storage service could do both bulk data ingest and streaming ingest

   The query services support UI, BQ command, and REST API

   The BigQuery Connectors to other services, such as Cloud Dataproc and Cloud Dataflow

   The storage service and the Query service work together to internally organize the data to make your queries and run efficiently on terabytes and petabytes. They even optimize your SQL statements syntax, whenever possible after you hit that Run Query button.