# Amazon_Vine_Analysis
Big Data using PySpark, Amazon Web Service (AWS), Google Colaboratory, and pgAdmin

## Overview of the Analysis
Various natural language processing skills were explored to prepare a customer review analysis for a client interested in digital video games.      

## Topics Explored
1. Define big data and describe the challenges associated with it.
2. Define Hadoop and name the main elements of its ecosystem.
3. Explain how MapReduce processes data.
4. Define Spark and explain how it processes data.
5. Describe how NLP collects and analyzes text data.
6. Explain how to use AWS Simple Storage Service (S3) and relational databases for basic cloud storage.
7. Complete an analysis of an Amazon customer review.

## Snapshot:
Using Google Colab and PySpark, we pulled review data from AWS into PG admin

![Pic 1](https://github.com/mpournaras/Amazon_Vine_Analysis/blob/main/resources/review_id_table.png?raw=true)

## Results

### How many Vine reviews and non-Vine reviews were there?

To consider:
* 792,113 total reviews.
* Only reviews with 20 or more votes where considered for the rest of the analysis leaving 18,739 reviews. 
* Helpful votes were defined as being 50% or greater than the total votes narrowing the list to 18,155 reviews.     
 
![Pic 2](https://github.com/mpournaras/Amazon_Vine_Analysis/blob/main/resources/vine_del3.PNG)  

**136** Vine reviews, **18,019** non-Vine reviews

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?     

![Pic 3](https://github.com/mpournaras/Amazon_Vine_Analysis/blob/main/resources/vine_del3_2.png?raw=true)  

**74** 5-star Vine reviews, **8482** 5-star non-Vine reviews

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?   

![Pic 4](https://github.com/mpournaras/Amazon_Vine_Analysis/blob/main/resources/vine_del3_3.png?raw=true)  

**54.41%** of Vine reviews were 5-stars
**47.07%** of non-Vine reviews were 5-stars

## Summary

Because the sample size was constricted to a degree that it was difficult to compare paid and unpaid Vine reviews, the analysis is biased towards unpaid Vine reviews.  Another indicator is comparing 47% of unpaid, 5-star Vine reviews to 54% paid, 5-star Vine reviews shows there is not as much bias. They are fairly equal with only 7% more reviews being 5-star when paid!

The starting criteria of 20 likes or the 50% helpful criteria may have been too high, which made the data set too small.  Adjustments to these criteria is a first step to reconsidering using this data set if we wanted to see if there was less bias
