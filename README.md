# Amazon Vine Analysis

## Project Overview 

This project will analyze reviews provided by the Amazon Vine program, which is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a fee to Amazon in addition to providing their products to Amazon Vine members. After receiving the product, members are required to publish a review. 

The analysis examines products within the "Health Personal Care" category. Usisng PySpark, data provided by Amazon Vine will undergo the ETL process, connecting to an AWS RDS instance and then loaded into pgAdmin. PySpark is used further to see if there is bias in the reviews from Vine members. 

## Results 

**How many Vine reviews and non-Vine reviews were there?**
There were 497 Vine reviews. There were 120,863 non-Vine reviews.

![image1](/images/1.png)

![image2](/images/2.png)

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?** 
220 Vine reviews had 5 stars. 74,470 non-Vine reviews had 5 stars. 

![image3](/images/3.png)

![image4](/images/4.png)

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
Of Vine reviews, 44.27% were 5 stars. Of non-Vine reviews, 61.62% were 5 stars.

![image5](/images/5.png)

![image6](/images/6.png)

## Summary

From the data provided, it seems that non-Vine members are more likely to give a 5 star rating than their Vine counterparts. This is supported by the percentage of non-Vine reviews that were 5 stars, 61.62%, in comparison to Vine reviews, of which only 44.27% were 5 stars. 

What is notable is that the dataset is not evenly distributed for each population. Non-Vine reviews make up 99.59%, while Vine reviews are only 0.41% of the data. However, from the description of the Vine program, it seems that Vine members are paid, regardless of the rating they give the product. If that is true, Vine membership may not cause bias.

Further analysis could examine product types by groupig reviews by a specific product. This category seems to include a range of products, which may have an effect on how people are providing reviews. An additional analysis could group further by company. Controlling for company may provide a more thorough analysis. If a specific company has more negative reviews, this could say more about the company quality than positivity bias. 