# Amazon_Vine_Analysis

## Overview of the analysis

The purpose of this project is pick one of Amazon datasest and use PySpark to perform the ETL process to extraxt the dataset transform the data, connect to an AWS RDS instance and load the transformed data into pgAdmin. In this case, we pick the Electronics dataset to perform this analysis. The next step is to use PySpark to determine if there is any bias toward favorable reviews from Vine members in this dataset. 

## Results:

### Filter the dataset where the total votes is equal to or greater than 20. 

<img width="715" alt="Screen Shot 2022-07-24 at 3 16 49 PM" src="https://user-images.githubusercontent.com/102264298/180664342-b22df272-a10d-4abc-b436-3107249b3dc9.png">

### Filter the dataset where the number of helpful votes divided by total votes is equal to or greater than 50%. 

<img width="968" alt="Screen Shot 2022-07-24 at 3 16 52 PM" src="https://user-images.githubusercontent.com/102264298/180664348-0bad39e6-03a1-4501-a107-d629ea13c5ed.png">

### Determine the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid).

![Screen Shot 2022-07-24 at 2 51 19 PM (2)](https://user-images.githubusercontent.com/102264298/180663513-79b14157-4bd3-46d9-b37e-a9b9cf9666d7.png)

* How many Vine reviews and non-Vine reviews were there?

  From the table above, we can see that there are 1080 Vine reviews and 49673 non-Vine reviews.

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

  There are 454 Vine reviews were 5 stars, while there are 23043 non-Vine reviews were 5 stars.

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

  The percentage of Vine reviews were 5 stars is 42.04%, while the percentage of non-Vine reviews were 5 stars is 46.39%. 

## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

From the analysis, there is not significant difference between the percentage of Vine reviews were 5 stars (42.04%) and the percentage of non-Vine reviews were 5 stars (46.39%). As a results, there is no positivity bias for reviews of Electronics in the Vine program. 
