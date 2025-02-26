# AI/ML Practical Assignment 1: Will the Customer Accept the Coupon?

## Summary (obtained from project description within ipynb file): 

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## Data (obtained from project description within ipynb file): 

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’.  There are five different types of coupons -- less expensive restaurants (under \$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\$20 - $50).

## Methods of observation: 

This project contains data cleaning methods of removing and replacing null data and columns, including removing the entire 'car' column as most of the data is missing. It contains multiple loc and query methods to filter out data further based on each observation criteria. Outputs are then compared in both text formats and different plots, to highlight the data science methodology learned in this course so far, and come up with conclusions for each data set. 

## Findings:

**Findings from Bar Coupons Offered:** 
1. Those who went to bars more than once a month are 24 percent more likely to accept coupons. 
2. Folks who are 25 years old and go to bars more often are 7 percentage points more likely to accept coupons. 
3. Folks who didn't have kids, worked in industries  
4. Folks who are lower income and go to cheap restaurants frequently are less likely to accept bar coupons
5. Folks who not widowed have a lower likelihood of accepting bar coupons even though they were sampled with folks going to the bar more than once a month

**Findings from Restaurants less than $20 Coupons Offered:** 
1. Age Data contains 21 and 46 year olds being the biggest sample sizes. Income data shows a fairly normal distribution, with the greatest number of sampled individuals residing within the 37500 - 49999 income bracket. 
2. As expected, we see the biggest acceptance ratio within the 21 year old age group, with the 26 year old age group following a similar trend, likely due to less disposable income. What is interesting is that there is a large acceptance ratio with the 46 year old age group as well, it's worth looking into other factors such as marital status and income level within that particular age group. 
3. As expected, we see the biggest acceptance ratio within the 12,500 - 24,999 income group, with income groups up to 75,000 dollars a year having reasonably high acceptance rates. High income groups such as over 87,500 dollars a year have an acceptance ratio of over 50 percent, but not as high as the lower to middle income groups.
4. There isn't much of a difference or a trend with the acceptance ratios of those who have children vs. those who do not. Income and age are believed to play a greater role in determining acceptance ratios.
5. Interestingly, for folks eat out at a restaurant less than 1 time a month, the acceptance ratio is significantly higher with no children, compared to folks with children.

## Path Forward: 
We have established trends which results in higher acceptance rates, compared to trends with seemingly no affect on coupon acceptance rates. Given the amount of variables in this data set, more research is needed into relationships between data sets, such as income level acceptance rates for drivers at the age of 46, and even how temperature, and the time of day affects the coupon acceptance rate. Given the findings, age, and frequency (amount of times going to a bar or a restaurant, similar to the coupon type), play a significant factor in whether the customer will accept the coupon. 
