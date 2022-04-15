# Amazon_Vine_Analysis
## Overview:
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

### Perform ETL on Amazon Product Reviews:  
Using your knowledge of the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame. You'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

## Results:

Using the amazon review data from [review](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz) (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz)

![Amazon_review_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/Amazon_review_df.png)
![review_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/review_df.png)
![customer_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/customer_df.png)
![product_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/products_df.png)
![vine_df](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/vine-df.png)

![review_id_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/review_table.png)
![customer_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/customer_table.png)
![product_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/product_table.png)
![vine_table](https://github.com/NishatSultana3538/Amazon_Vine_Analysis/blob/main/image/vine_table.png)


