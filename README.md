# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program:

This project included the analyzing Amazon reviews written by members of a paid Amazon Vine program or other reviewers to determine if there is any bias for favorable reiews by the reviewers in the Amazon Vine Program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 

The goal of this project was to use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, PySpark was used to determine if there is any bias toward favorable reviews from Vine members in the dataset. The [Amazon Watch dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Watches_v1_00.tsv.gz) was used in the dataset. 

Programming Tools:
- 
- Amazon AWS RDS Instance
- pgAdmin 4 (Prostgres SQL 14.2)
- pySpark
- Google Colab Notebook

## Results:

There is a bulleted list that addresses the three questions for unpaid and paid program reviews (7 pt)
Deliverable 3: A Written Report on the Analysis (20 points)\



![watch-customers](/images/watch-customers.png)

![watch-products](/images/watch-products.png)

![watch-reviews](/images/watch-reviews.png)

![watch-vine](/images/watch-vine.png)

![pgSQL-customers](/images/pgSQL-customers.png)

![pgSQL-products](/images/pgSQL-products.png)

![pgSQL-review-id](/images/pgSQL-review-id.png)

![pgSQL-vine,png](/images/pgSQL-vine,png.png)

![watch-vine-recreated](/images/watch-vine-recreated.png)

![total_votes_over20](/images/total_votes_over20.png)

![helpful_votes_over_50perct](/images/helpful_votes_over_50perct.png)

![watches-vine-paid](/images/watches-vine-paid.png)

![watches-vine-paid-describe](/images/watches-vine-paid-describe.png)

![watches-vine-unpaid](/images/watches-vine-unpaid.png)

![watches-vine-unpaid-describe](/images/watches-vine-unpaid-describe.png)

![vine-paid-counts](/images/vine-paid-counts.png)

![vine-unpaid-counts](/images/vine-unpaid-counts.png)


Results: Using bulleted lists and images of DataFrames as support, address the following questions:
**How many Vine reviews and non-Vine reviews were there?**
- There were 47 vine reviews and 8362 non-Vine reviews

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
- There were 15 Vine reviews
- There were 4332 non-Vine reviews

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
- 31.9% of Vine reviews were 5 stars
- 51.8% of non-Vine reviews were 5 stars

## Summary: 
In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

This analysis showed that there was no bias towards favorable reviews by the paid Vine program. 


Summary:
The summary states whether or not there is bias, and the results support this statement (2 pt)
An additional analysis is recommended to support the statement (2 pt)

Vine Reviews
Total votes for 5 stars = 570
Total number of votes = 2252
% 5-Star Vine votes = 25.35%

Non-Vine Reviews
Total votes for 5 stars = 216,295
Total number of votes = 394,223
% 5-Sta Non-Vine votes = 54.9%

