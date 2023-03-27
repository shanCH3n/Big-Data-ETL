# Big-Data-ETL

## Background
The primary goal of this project was to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. Data from Amazon's publicly available product reviews were used. Amazon product review datasets are quite large and can exceed the capacity of local machines. Thus, Google Colab was used to facilitate the process.


## Part 1
Two separate Amazon customer review datasets, one for watches and the other for outdoor equipment, were selected for the ETL process. The code that was used to extract the data, transform each into four DataFrames, and load the DataFrames into an RDS instance can be found in the following notebooks: part_one_watches.ipynb and part_one_outdoors.ipynb. 

Four dataframes were created for each customer review dataset - with a total of 8 created and uploaded onto Amazon Web Services (AWS)'s RDS. These are labeled according to the product they represent (e.g., watches_review_id_table; outdoors_customers).

Here is a summary of the contents and columns of each dataframe.  
- _review_id_table: 'review_id', 'customer_id', 'product_id', 'product_parent', 'review_date'.
- _products: 'product_id', 'product_title'.
- _customers: 'customer_id', 'customer_count'.
- _vine_table: 'review_id', 'star_rating', 'helpful_votes', 'total_votes', 'vine'.


## Technologies used:
- Cloud Computing (Google Colab)
- PySpark
- AWS RDS Database
- AWS S3 Buckets
- SQL (PostgresSQL & pgAdmin)


## References
Amazon Customer Reviews Dataset. (n.d.). Retrieved March 27, 2023, from: https://s3.amazonaws.com/amazon-reviews-pds/readme.html
