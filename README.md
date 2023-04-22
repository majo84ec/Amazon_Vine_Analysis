# Amazon_Vine_Analysis

## Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project,we will pick one of datasets reviews and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

## Results:

### Paid:

![image](https://user-images.githubusercontent.com/120151872/233803685-067ec17c-fc44-4f4d-bfb1-26c30fe7d2bf.png)

### Unpaid:

![image](https://user-images.githubusercontent.com/120151872/233803777-dd884761-ce29-46ed-b6af-be295d09122f.png)

Grocery dataset was used for this analysis. The total number of reviews was 28348 where 21 were paid and 28287 unpaid. The number of members who give 5 starts were 15909  (20 paid, 15689 unpaid), and the percentage of 5 starts reviews were higher in unpaid category with 55.46% compare with 32.78% of paid. 

### Summary
Based on the results, Vine members did not show bias when rating their products considering the 32.7% gave 5 stars-Vine. However, the total reviews  in each category are different ,so in order to support this assumption we should  important to considerate same analysis with other datasets.
In addition it would be appropiate to compare 1 star reviews from both Vine and non-Vine members to further support this conclusion.
