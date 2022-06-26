# Amazon_Vine_Analysis

## Overview of the analysis of the Vine program:

This project included the analyzing Amazon reviews written by members of a paid Amazon Vine program or other reviewers to determine if there is any bias for favorable reiews by the reviewers in the Amazon Vine Program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 

The goal of this project was to use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, PySpark was used to determine if there is any bias toward favorable reviews from Vine members in the dataset. The [Amazon Watch dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Watches_v1_00.tsv.gz) was used in the dataset. 

Programming Tools:
- Amazon AWS RDS Instance
- pySpark
- pgAdmin 4 (Prostgres SQL 14.2)
- Google Colab Notebook
- Git

## Results:

The ETL process of the Amazon Watches Reviews data (Amazon Watches Reviews) was performed in Google Colab Notebooks using pySpark. Figures 1 - 4 show the tables for customers, products, reviews, and vine reviews, respectively, after extracting and transforming data from the tsv file for Amazon "Watches" reviews. Figures 5 - 8 show the screenshots of SQL output after loading data into SQL tables in the Amazon AWS RDS instance. Figures 9 - 11 show dataframes for re-created vine table and it cleaning up stages. Figure 12 - 13 show final tables for Vine reviews and some statistics, respectively. Figure 14 - 15 show final tables for Non-Vine reviews and some statistics, respectively. Figure 16 and Figure 17 sho the review counts for Vine Reviews and Non-Vine reviews, respectively.  

**How many Vine reviews and non-Vine reviews were there?**
- There were 47 vine reviews and 
- There were 8362 non-Vine reviews

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
- There were 15 Vine reviews
- There were 4332 non-Vine reviews

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
- 31.9% of Vine reviews were 5 stars
- 51.8% of non-Vine reviews were 5 stars


![watch-customers](/images/watch-customers.png)

**Figure 1.** Screen shot showing customer table dataframe in pySpark (in Google Colab Notebook)

![watch-products](/images/watch-products.png)

**Figure 2.** Screen shot showing products table dataframe in pySpark (in Google Colab Notebook)

![watch-reviews](/images/watch-reviews.png)

**Figure 3.** Screen shot showing reviews table dataframe in pySpark (in Google Colab Notebook)

![watch-vine](/images/watch-vine.png)

**Figure 4.** Screen shot showing vine table dataframe in pySpark (in Google Colab Notebook)

![pgSQL-customers](/images/pgSQL-customers.png)

**Figure 5.** Screen shot showing customers table in pgAdmin

![pgSQL-products](/images/pgSQL-products.png)

**Figure 6.** Screen shot showing products table in pgAdmin

![pgSQL-review-id](/images/pgSQL-review-id.png)

**Figure 7.** Screen shot showing reviews table in pgAdmin

![pgSQL-vine,png](/images/pgSQL-vine,png.png)

**Figure 8.** Screen shot showing vine table in pgAdmin

![watch-vine-recreated](/images/watch-vine-recreated.png)

**Figure 9.** Screen shot showing recreated vine dataframe (in Google Colab Notebook)

![total_votes_over20](/images/total_votes_over20.png)

**Figure 10.** Screen shot showing table after filtering for total votes >= 20 (in Google Colab Notebook)

![helpful_votes_over_50perct](/images/helpful_votes_over_50perct.png)

**Figure 11.** Screen shot showing table after filtering for thelpful votes/ total votes >= 50% (in Google Colab Notebook)

![watches-vine-paid](/images/watches-vine-paid.png)

**Figure 12.** Screen shot showing table for paid Vine reviews (in Google Colab Notebook)

![watches-vine-paid-describe](/images/watches-vine-paid-describe.png)

**Figure 13.** Screen shot showing some statistics for Vine reviews (in Google Colab Notebook)

![watches-vine-unpaid](/images/watches-vine-unpaid.png)

**Figure 14.** Screen shot showing table for Non-Vine reviews (in Google Colab Notebook)

![watches-vine-unpaid-describe](/images/watches-vine-unpaid-describe.png)

**Figure 15.** Screen shot showing some statistics for Non-Vine reviews (in Google Colab Notebook)

![vine-paid-counts](/images/vine-paid-counts.png)

**Figure 16.** Screen shot showing review counts for paid Vine reviews (in Google Colab Notebook)

![vine-unpaid-counts](/images/vine-unpaid-counts.png)

**Figure 17.** Screen shot showing review counts for Non-Vine reviews (in Google Colab Notebook)

## Summary: 

In summary, the analysis of reviews for watches shows that there is no positivity bias in the paid Vine program because % 5-star reviews for Non-Vine reviewers (52%) were higher compared to that of Vine Program reviewers (32%). 

An additional analysis was performed using the sum of votes for Vine reviews and Non-Vine reviews. Figure 18 - 19 show results for Vine reviews whereas Figure 20 - 21 show results for Non-Vine reviews. 

Vine Reviews
- Total votes for 5 stars = 570
- Total number of votes = 2252
- % 5-Star Vine votes = 25.35%

Non-Vine Reviews
- Total votes for 5 stars = 216,295
- Total number of votes = 394,223
- % 5-Star Non-Vine votes = 54.9%

This analysis is also in agreement with the previous analysis demonstrating that there is no positivity bias in the Vin program.

![5star-total-vine-votes](/images/5star-total-vine-votes.png)

**Figure 18.** Screen shot showing total 5-star votes for paid Vine reviews (SQL pgAdmin)

![total-vine-votes](/images/total-vine-votes.png)

**Figure 19.** Screen shot showing total votes for paid Vine reviews (SQL pgAdmin)

![5star-total-non-vine-votes](/images/5star-total-non-vine-votes.png)

**Figure 20.** Screen shot showing total 5-star votes for Non-Vine reviews (SQL pgAdmin)

![total-non-vine-votes](/images/total-non-vine-votes.png)

**Figure 21.** Screen shot showing total votes for Non-Vine reviews (SQL pgAdmin)

