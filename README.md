# Big_Data_AWS


##  Overview of the Analysis
The objective of this assignment was to conduct a customer review analysis for digital video games using ETL (Extract, Transform, Load) strategies. Data was gathered from AWS and processed using Google Colaboratory and the PySpark plugin. The analysis was performed to meet the needs of a client seeking insights into customer reviews.
![pyspark import 1](https://user-images.githubusercontent.com/112728628/216843050-f441ce79-992f-4ec6-9955-9ce62836c4c8.PNG)

![pgadmin](https://user-images.githubusercontent.com/112728628/216843006-cfb10c78-f9ce-4d4c-9fed-40431599fdad.PNG)

##  Results
How many Vine reviews and non-Vine reviews were there?
- The data set contained over 140,000 reviews.
![paid and unpaid program](https://user-images.githubusercontent.com/112728628/216843034-c4addd9f-d64c-44d4-b841-d2f6b1a09a0f.PNG)

- Products with 20 or more votes were selected as the primary focus of the analysis, resulting in 3,342 reviews meeting this criteria. To clean up the data set, only
reviews rated as helpful (50% or more of total votes) were used, resulting in 1,685 reviews.
![50 percent helpful votes](https://user-images.githubusercontent.com/112728628/216843040-500a8f8a-736c-4552-a5eb-798dc98a8a02.PNG)
![20 total votes](https://user-images.githubusercontent.com/112728628/216843046-6243af0d-4600-42f9-a8bb-c9c5d7b9cfd1.PNG)

- However, applying the helpful review criteria had a drawback. The sample size became too small, and as a result, there were no paid Vine reviews in the data set. On the other hand, the non-Vine paid program showed better results for 5-star ratings.

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
-  After filtering for helpful reviews, a filter was added to separate the paid and non-paid programs and grab only the 5-star rated reviews. Out of the 1,685 helpful reviews, 631 were 5-star reviews. 631 of these were for the unpaid Vine program while there were no 5-star reviews for the paid Vine program.

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- As there were no paid Vine reviews, no calculations were performed to avoid zero division errors.

- The percentage of 5-star reviews for the unpaid Vine program was 37.44%.

![percentage](https://user-images.githubusercontent.com/112728628/216843020-ebe3c6d4-7419-4342-a93b-9e32d694d853.PNG)



##  Summary
The limited sample size resulted in an inability to compare paid and unpaid Vine reviews accurately, causing bias towards unpaid Vine reviews. This is evident in the difference between 37% of 5-star reviews for unpaid Vine and 0% for paid Vine. To address this issue, adjusting the starting criteria of 20 likes or the 50% helpful threshold may be necessary to increase the size of the data set and make it more useful.
