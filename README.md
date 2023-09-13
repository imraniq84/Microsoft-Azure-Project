# Microsoft-Azure-Project

This is a Microsoft Azure Profile Project created by me and the idea is to upload Covid.xlsx in the datalake storage gen 2 and create a pipeline in Azure synapse to convert xlsx format to parquet.

(Parquet is optimized to work with complex data in bulk and features different ways for efficient data compression and encoding types. This approach is best especially for those queries that need to read certain columns from a large table)
Then using Azure synapse, Apache spark pool is created that would allocate resource to notebook which would be used to read the parquet file , create database and tables to perform aggregation functions on the file which is then saved on lake database.

Separate serverices could have been used such as Azure datalake storage gen 2 , Azure data factory, Data bricks, but instead Azure datalake storage gen 2 and Azure synapse have been used as it contains all the services needed to use on a single platform.
