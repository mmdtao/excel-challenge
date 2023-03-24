# Kickstarting with Excel

## Overview of Project

### Purpose
Given data regarding Kickstarter campaigns, what trends can we determine will lead to successful, failed, or canceled campaigns using pivot tables and descriptive statistics. Specifically, Outcomes based on Launch Date and Outcomes based on Goals should be analyzed.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Using a pivot table to sort by launch date, I set the rows to  "Date Created Conversion" with "Parent Category" and "Years" as categories which allows both a broad analysis by month but can be further analyzed by looking at trends each year by activity. As shown in the "Outcomes Based on Launch Date" graph below, it is clear that the highest percentage of successful campaigns were launched in June, July, and September. These campaigns were roughly 61-63% successful. The graph also suggests to avoid starting campaigns in December and August which had success rates at or below 50%. 

<img width="480" alt="Outcomes Based on Launch Date" src="https://user-images.githubusercontent.com/114324871/227411563-e4133656-18b5-453f-9a8d-8719272c7530.png">


### Analysis of Outcomes Based on Goals
To create tables showing outcomes based on goal increments, I needed to use the COUNTIFS function to pull specific ranges of goals from the datasheet, each time adjusting the limits to the corresponding goal bracket. An example of the COUNTIFS formula I used is shown below:

<img width="795" alt="Sample Code" src="https://user-images.githubusercontent.com/114324871/227414523-5d7561c5-841e-4f4b-a798-ff7891885c19.png">

As shown in the "Outcomes Based on Goals" graph below, the most successful goals set for kickstarter campaigns are the $15,000-$19,999, $20,000-$24,999, and $30,000-$34,999 ranges. These three ranges were 100% successful. Campaign targets that had a success rate below 50% included the $10,000-$14,999 and >$50,000 ranges. Those ranges and $5,000-$9,999 are probably the ranges to avoid due to failure or cancelation. 

<img width="899" alt="Outcomes Based on Goals" src="https://user-images.githubusercontent.com/114324871/227411594-0f9fb8a4-80bc-4472-8f8c-3672ae3b6d66.png">


### Challenges and Difficulties Encountered

## Results

- What are some limitations of this dataset?

From the descriptive statistics, there are a fair amount of outliers suggesting that this is not a normally distributed dataset. Since the mean is greater than the median for both "successful" and "failed" campaigns, it suggests that to have a more successful campaign you would need to have a larger amount of backers than in reality. The summary statitics also showed there was much more variance in "successful" campaigns which makes sense as "failed" campaigns have no lower limit while a "successful campaign" technically has no upper limit.
<img width="859" alt="Outcomes Whiskerplot" src="https://user-images.githubusercontent.com/114324871/227413344-ac8e4ffa-e87b-4e36-a008-92827a3a5eea.png">

- What are some other possible tables and/or graphs that we could create?

I think a graph showing sub-category success by month would be helpful in determining whether there are more activity-specific trends throughout the year. For example, will the data suggest that people are not thinking about plays in early spring when people tend to shift their activities outdoors? Another graph comparing goal amounts and months could show trends in which the population tends to be more altruistic.
