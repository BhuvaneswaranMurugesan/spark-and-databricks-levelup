# RDD

Resilent Distributed Dataset, which is Sparks fundamental low level Datastructure and Dataframes are build on top of that.

RDD don't contains Catalyst Optimizer where Dataframe and Dataset contains Catalyst Optimizer

## Dataframe vs Dataset

- Dataset is Typed API, and it has class to maintain strict datatype , eg: Dataset[T]
- Dataset is only available in java and Scala not available in pyspark

where as Dataframe is row, Dataset[Row] which is available in spark.

# Managed vs External Tables

- Databricks Manage both actual Storage and metadata data
- External Table hold only metadata in databricks

example: if you drop both actual and external table , the actual data is lost where as actual data of external table is located in some external storage like s3 bucket etc.

Data governance: unity catalog controls everything in databricks, for external table flexible but requires discipline

# Unity Catalog