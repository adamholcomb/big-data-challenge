# Big Data



## Background

In this assignment I put your ETL skills to the test. Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. However, they are quite large and can exceed the capacity of local machines to handle. One dataset alone contains over 1.5 million rows; with over 40 datasets, this can be quite taxing on the average local computer. My first goal will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

Goal: Create DataFrames to match production-ready tables from two big Amazon customer review datasets.

- - -

## Procedure

* Use a schema to create tables in the RDS database through Postgres.

* Create two separate Google Colab notebooks and extract two datasets from the list at [review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), one into each notebook. File 1 uses video game reviews and file two uses music reviews.

* These files are tab separated and have a header.

* For each notebook (one dataset per notebook), the following is completed:

  * Count the number of records (rows) in the dataset.
  * Drop NA values
  * Count rows again
  * Transform the dataset to fit the tables in the Postgres schema. 
  * Cast the data types to match the schema.
  * Load the DataFrames that correspond to tables into an RDS instance.