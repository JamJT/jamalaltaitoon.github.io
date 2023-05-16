---
layout:  post
title:  "Airbnb Analysis: Venice, Italy"
author:  Jamal AlTaitoon
image:  
---
Case Situation:
We were approached by a couple of investors hoping to invest in properties in Venice, Italy to turn into Airbnb properties for consultation and analysis. They want to know where to invest, what type of property, and what type of strategy to use for investment to have the highest ROI.

Method:
To start our analysis, we used data scraped from Airbnb website relating listings located in Venice, Italy. Before we started cleaning the dataset, we had a quick look across the dataset and data dictionary to see which features and observations are pertinent to the scope of the analysis. 
1.	Used Conditional Formatting to filter out any duplicates that might exist. There were no duplicates.
2.	Replaced Null values in (review_scores_rating) column with the average rating of all listings.
3.	Replaced Null values in (reviews_per_month) column with 0 value since absence of number of reviews in this case means zero reviews were given for the listing.
4.	Removed 52 unnecessary features from the dataset for a clearer analysis.
5.	Added 3 new features to the dataset using other existing features.
6.	Created the (booked_nights) column to find out how many nights the property has been booked. To achieve this, we multiplied column (number_of_reviews_ltm) by column (minimum_nights)
7.	Created the (revenue) column to find out how much the property is making by multiplied column (price) by column (booked_nights).
8.	Created the (individual_company) column to find out if the listings are operated by individuals or companies using the (instant_bookable) column which is an indicator of commercial owned property if true.
9.	Deleted 3 listings from the dataset (ID numbers: 42279260, 43205683, and 45683814) which had $0 as price, making them unnecessary for the analysis.
10.	Generated Pivot Tables to find out:  
a.	Which neighborhoods host the most listings?  
b.	What property types receive the most positive reviews?  
c.	How much revenue do successful hosts generate?  

11.	Using Pivot Tables, we created visualizations to rank:
   a.	The neighborhoods by number of listings.  
   b.	The neighborhoods by average rating score.  
   c.	The property types by number of listings.  
   d.	The property types by average rating score.  
   e.	The property types by average revenue.  
   f.	The hosts by total revenue.  

