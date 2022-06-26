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
Deliverable 3: A Written Report on the Analysis (20 points)

Deliverable 3 Instructions

For this part of the Challenge, you’ll write a report that summarizes the analysis you performed in Deliverable 2.
The report should contain the following:
Overview of the analysis: Explain the purpose of this analysis.
Results: Using bulleted lists and images of DataFrames as support, address the following questions:
How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
Deliverable 3 Requirements

Structure, Organization, and Formatting (6 points)

The written analysis has the following structure, organization, and formatting:
There is a title, and there are multiple sections (2 pt)
Each section has a heading and subheading (2 pt)
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (14 points)


Summary:
The summary states whether or not there is bias, and the results support this statement (2 pt)
An additional analysis is recommended to support the statement (2 pt)
