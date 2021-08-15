# Amazon_Vine_Analysis

## Overview

The purpose of this project was to analyze reviews on Amazon for sports products and determine whether Vine members show bias by providing positive reviews. ETL was conducted on the dataset to extract it, transform the data, and load it into pgAdmin. Afterwards, the data was analyzed using pandas.

To view the ETL code, click [here](https://github.com/fadlnabbouh/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb). 

To view the analysis, click [here](https://github.com/fadlnabbouh/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb).

## Results

To determine whether bias exists with Vine-member reviews and sports products, the original data was transformed into a table in pgAdmin with review_id, rating, helpful votes, total votes, verified purchase, and vine data. Only products with 20 votes or more were analyzed and of that data, only ones where helpful votes made up 50% or more of total votes were analyzed.The dataframe was then split into two dataframes to represent vine and non-vine members.

![image1](https://github.com/fadlnabbouh/Amazon_Vine_Analysis/blob/main/resources/image1.png)

From the analysis, I found that for sports product reviews on Amazon:
- 311 reviews were from vine members
- 57509 reviews were from non-vine members
- of the 311 reviews from vine members, 129 were 5 star reviews or 41.48%
- of the 57509 reviews from non-vine members, 30631 were 5 star reviews or 53.26%

![image2](https://github.com/fadlnabbouh/Amazon_Vine_Analysis/blob/main/resources/image2.png)

## Summary

In summary, 53.26% of non-vine member reviews were 5 star, while only 41.48% of vine member reviews were 5-star. This shows that, with sports products on amazon, there is no bias towards leaving a high rated review. 

Additional analyses should be conducted to determine whether a bias exists, however. Sports products may very well be great products that warrant a high rated review. A future analysis that I would conduct is to compare the proportion of 5 star rated reviews between vine and non-vine members across multiple types of products. In addition, I'd also analyze proportion of other ratings (4-star ratings are also decent ratings while analyzing 1-star ratings may help determine if there is a bias towards not leaving a low review).
