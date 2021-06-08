# Amazon_Vine_Analysis


## Overview of Analysis

The purpose of this analysis is to use the knowledge gained from this module of the cloud ETL process and create an AWS RDS database with tables in pgAdmin. There are approximately 50 different datasets, each one containing reviews of a specific product, to choose from. I decided to use the "Mobile Electronics" dataset for my analysis. With this dataset, PySpark will be used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and then load the transformed data into pgAdmin. PySpark was then used again to analyze Amazon reviews written by members of the paid Vine program and can be used to determine if there are any bias toward favorable reviews form Vine members from the selected dataset. 


## Results

### How many Vine reviews and non-Vine reviews were there?
  
![total](https://user-images.githubusercontent.com/75760493/121084590-71a3f080-c7a6-11eb-89ae-1b81138546b4.PNG)

From the executed code above, it shows that there were only 4 Vine reviews compared to 1064 non-Vine reviews.


### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![five star](https://user-images.githubusercontent.com/75760493/121083715-613f4600-c7a5-11eb-91d4-514611f10de1.PNG)
  
From the executed code above, it shows that there were only 1 5 star Vine review compared to 527 5 star non-Vine reviews. 


### What percentage of Vine reviews were 5 star? What percentage of non-Vine reviews were 5 star?

![percentage](https://user-images.githubusercontent.com/75760493/121084748-a57f1600-c7a6-11eb-8094-0a9195a7766d.PNG)

From the executed code above, it shows that only 25% of the Vine reviews were 5 stars compared to 49.53% of non-Vine reviews being 5 stars.


## Summary

What the results seem to suggest is that the Vine reviews have a smaller percentage of 5 star reviews (25%) compared to the percentage of non-Vine 5 star reviews (49.53%). The Amazon Vine program is a program where the most trusted reviewers on Amazon are invited to post reviews on new and pre-released items to help provide feedback that will assist other customers in making informed purchase decisions. Amazon only invites reviewers that have a high reviewer rank, which is based on the quality and helpfulness of all their reviews. Based on the criteria needed to be invited to the Amazon Vine program, it seems that the reviewers they select are credible in Amazon's eyes to review these new products. From the 5 star reviews for the Vine and non-Vine reviews, there doesn't seem to be any sign that there is a bias towards favorable reviews from Vine members. The results show that the Vine members are less likely to rate something as a 5 star then non-Vine members. From this dataset, it appears that Vine members are more critical of what they review instead of showing a favorable bias to what they review. 

There is one issue with this dataset that makes the previous conclusion difficult to justify; and that is that there was a significantly smaller sample size of Vine reviews compared to non-Vine reviews. There were only 4 Vine reviews compared to 1064 non-Vine reviews. A sample size of 4 can't be depended on to give accurate metrics, especially when comparing it to a sample size of 1064. So even though the results show there is no favorable bias from Vine members, it would require a larger size of data to determine if there is or isn't favorable bias. Unfortunately, this dataset doesn't give enough data to make a proper analysis of the Vine reviews. 

