# Amazon_Vine_Analysis
## Overview:
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. 
### Analysis Overview:
This project analyzes Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.

### Perform ETL on Amazon Product Reviews:  
Using your knowledge of the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame. You'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

## Resources:
Data Source: Amazon Review datasets.
Software: Google Colab Notebook, PostgreSQL , pgAdmin 4, AWS

## Results:

Using the amazon review data from [review](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz) (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz) and the Google colab notebook file [Amazon_review-ETL](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)
I fot the following data frame:

![Amazon_review_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/Amazon_review_df.png)

![review_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/review_df.png)

![customer_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/customer_df.png)

![product_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/products_df.png)

![vine_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/vine-df.png)

After creating the connection to the AWS RDS instance(database))
and loading the DataFrames  to tables in pgAdmin I got the following tables:

![review_id_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/review_table.png)

![customer_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/customer_table.png)

![product_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/product_table.png)

![vine_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/vine_table.png)


## Summary:
51% of the Vine reviews  were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program or the paid program.
We could also analyze the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.

