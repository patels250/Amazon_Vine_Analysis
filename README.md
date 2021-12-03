# Amazon_Vine_Analysis

## Project Overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Here we run analysis on Amazon's Health & Personal Care Review Dataset to determine if there is any positivity bias in reviews written by members of the paid Amazon Vine program.

## Results

- We filtered the dataset down to reviews with more than 20 votes to focus our analysis on the most popular reviews. We then filtered the resulting reviews to those who received a helpful rating greater than or equal to 50%. This resulted in 114,313 reviews for our data set. 
- Of the helpful reviews, only 475 are paid Vine Program reviews. With non-Vine reviews making up 113,838 of the dataset:  
- There are a total of 71,951 5 Star reviews in the dataset, accounting for 62.94% of the reviews. 
- Of the Vine reviews, 45.05% of them were 5 Stars. While 61.76% of non-Vine reviews were 5 Stars. 

## Summary

There is no evidence to suggest that the Vine reviews contain any positivity bias. Non-Vine reviews make up over 99% of the reviews in the data set and also account for 61.76% of the 5 star reviews. The Vine reviews only have a 5 Star percentage of 45.05%.

What the current dataset doesn't share is if the product is new to the reviewer or one the reviewer has used regularly for years. This is important with Health and Personal Care products that require ongoing use to observe real results. Vine reviewers may be more critical of Health and Personal Care products than unpaid reviewers because the product may be newly introduced to them, whereas non-Vine reviewers are selecting products and brands they trust. This analysis would be more useful if we used Natural Language processing to extract information from the content of the review. We could classify specific words that indicate if the review reveals the product is new to the reviewer or not. To do so, I would create a dataFrame filtered by classified text and compare it to non-classified text to determine if this reveals any positivity bias.