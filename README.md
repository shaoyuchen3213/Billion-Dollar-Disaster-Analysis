# Billion-Dollar-Disaster-Analysis
Analysis recently 20 year the amount and death in Disaster.
Main Questions: 
Does different types of disaster have different levels of impact monetarily and deathly? 
What is the main cause of cost in a disaster? 
Does duration and number of deaths contribute to the cost?

Importance Of The Question: 
After we know the contributor of the cost, we can predict how much a disaster would cost and help insurance companies make decision on the costs of their insurance


This dataset holds 12 columns and 338 rows of information on 7 disasters.  This project analyses the deaths, duration, and cost of each disaster. 

Preview of the first 5 rows of our dataset using the .head() function.

![1671514806065](https://user-images.githubusercontent.com/35966970/208592203-00114f27-aad0-40a3-a125-4c5f2927392c.jpg)

How are different disasters distributed each year?
We use the pivot function, and set index equal to 'begin year’, which is xlabel, and use the .grid() function to configure the grid lines.
![1671514902037](https://user-images.githubusercontent.com/35966970/208592434-b2ad3685-1a3d-4e88-b897-91f40b53be51.jpg)


Regression Analysis
We use ‘Deaths’ and our new variable ‘Duration’ as X and set the new variable ‘Amount’ as our Y because the objective is to analyze correlations between these three variables by running the stats model.

From the OLS Regression Result, there is a strong correlation between Death and Amount, which means the deadlier the disaster is, the more costly it can make. 

In contrast, with a p-value greater than 0.05, Duration has no significant impact on the Amount.

![1671514985471](https://user-images.githubusercontent.com/35966970/208592570-c10f0072-b00e-43b1-8a85-2fb56c6c342b.jpg)


Because the trend of disaster occurrence is increasing, the market demand for disaster insurance is considerable. Insurance companies should consider adding disaster insurance to product items.

The number of Severe Storm occurrences per year is increasing at an alarming rate, and the number of deaths is relatively low, so it is a high-demand and profitable item.

Companies that already have disaster insurance as their product should increase the price of disaster insurance in Tropical Cyclone. It is a highly risky item with a short duration and the largest number of deaths.

More disasters occur in Spring and Summer, so companies should consider increasing prices in these two seasons.



