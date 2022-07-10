# Amazon_Vine_Analysis

## Overview
The Amazon Vine program is a paid service that allows manufacturers and publishers to receive review for their products. Amazon Vine members are provided products from companies and are required to publish a review. Out of about 50 different datasets that contained reviews for multiple different products ranging from clothing apparel to wireless products, I chose to focus my analysis on video games. 

In order to determine if there's any bias toward favorable reveiws from Amazon Vine members, I utilize PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data in n pgAdmin. 

## Results
* To start my analysis, I filtered by reviews with more than 20 votes and those that had more than 50% helpful votes.
<img width="682" alt="Filtered helpful" src="https://user-images.githubusercontent.com/100165760/178156458-81de8627-6949-49be-8421-bbaf16ced964.png">

From the dataset above, calculations were created to identify:
* how many paid vs unpaid reviews there were
* the number of 5-star reviews
* the percentage of 5-star review for Vine and non Vine reviews

Please see the images below:
<img width="685" alt="review" src="https://user-images.githubusercontent.com/100165760/178156724-30d68f53-f232-4c12-9321-d87b74bea730.png">
<img width="766" alt="percentages" src="https://user-images.githubusercontent.com/100165760/178156765-e494d881-1383-4219-ab30-4920cadac8f6.png">
