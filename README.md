<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/Vine-Header.png">

# Analysis of Amazon Vine Reviews

## Overview
Ratings quality is only growing in importance. Because of the growth of ratings platforms and
consumers' desires to get the most value for thier money, many companies both rely on good
ratings from third party websites and from reviews on their own sites. Amazon is the top retail e-commerce company
in the US, so their reviews are widely consulted and, to protect consumers, should be unbiased.

Amazon's <a href="https://www.amazon.com/gp/vine/help">Amazon Vine</a> program is an invitation only 
review program that the company claims "invites the most trusted reviewers on Amazon to post opinions 
about new and pre-release items to help their fellow customers make informed purchase decisions." 
While Vine Voices are not paid in cash for their reviews, they are paid by being provided with 
<a href="https://tinuiti.com/blog/amazon/amazon-vine-program/">"free products that have been submitted 
to the program by participating vendors."</a> It is important, therefore, to test for possible bias on 
the part of their reviewers (Amazon Voices). We can initially test for bias by comparing the reviews of 
Amazon Vine reviewers and non-paid Amazon reviewers on the Amazon platform.

The analysis here examines the reviews of video games on the Amazon platform.

Resources Used:
- Amazon RDS
- Postgres/pgAdmin
- Google Colab
- PySpark

## Results
Looking at the relationship between 5-star reviews from Amazon Vine members and the non-paid reviewers,
we see a significantly higher percentage of 5-star reviews from Amazon Vine members. Amazon Vine members
gave products a 5-star rating 51.06% of the time, while non-paid reviewers gave products
a 5-star review 38.70% of the time.

- ### How many Vine reviews and non-Vine reviews were there?
#### Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/total_paid_reviews.png"><br>

#### Non-Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/total_unpaid.png"><br>

- ### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
#### 5-Star Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/total_paid_5-star.png"><br>

#### 5-Star Non-Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/totao_unpaid_5-star.png"><br>

- ### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
#### Percentage of 5-Star Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/percentage_paid_5-star.png"><br>

#### Percentage of 5-Star Non-Vine Reviews
<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/percentage_unpaid_5-star.png"><br>

## Summary
1. Is There a Bias?
This analysis would indicate a positivity bias on the part of Amazon Vine members.

2. Additional Analysis
The number of Amazon Vine reviewers (94) is significantly smaller than the number of non-paid 
reviewers (40,471). It would be important to compare the measures of central tendency for the
two groups to further clarify any bias.

3. Finally, these analyses should be performed for the other review areas (i.e., other than 
the video games analyzed here) to test for bias across the Amazon Vine platform.


<img src="https://github.com/tn64/Amazon_Vine_Analysis/blob/main/Resources/pexels-lalesh-aldarwish-194511.png">
<!-- Photo by lalesh aldarwish from Pexels -->
