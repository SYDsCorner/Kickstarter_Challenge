# Kickstarter_Challenge
Analyses: outcomes based on launch date and on goals

## Overview of Project

### Purpose
   Louise’s play Fever came close to its fundraising goal in a short amount of time. This analysis would help Louise visualize how the different campaigns fared compared to hers in relation to their launch dates and their funding goals.

## Analysis and Challenges

### 1. Analysis of Outcomes Based on Launch Date

- First, I created the new column to extract the year from the “Date Created Conversion” column by using the YEAR() function on column U.

![Years_Column U](https://user-images.githubusercontent.com/89308251/131071751-ea3633d4-f2d8-4b81-9883-6e383a5ac6f6.png)

- Then, I created the pivot table where I can show Louise the data she wants to compare by filtering by “Parent Category” and “Years”, columns with “outcomes”, rows with “Date Created Conversion”, and values with “Count of outcomes"

    > I also filtered and sorted the column labels to show only “successful”, “failed”, and “canceled” in order to make it easier to read.
Finally, I created the line chart from the pivot table to visualize and compare between outcomes and launch month.

![PivotTable_and_Chart_Outcomes_vs_Launch](https://user-images.githubusercontent.com/89308251/131071837-2a53199a-64fb-4087-84a8-af388c0aaa17.png)



### 2. Analysis of Outcomes Based on Goals

- First, I created a new sheet to hold the data I needed on the chart. 

- Second, I used COUNTIFS() functions to populate the "Number Successful," "Number Failed," and "Number Canceled" columns. 

- Third, I used the SUM() function to populate the “Total Project” column with the number of successful, failed, and canceled projects. 

- Forth, I calculated the percentage of successful, failed, and canceled projects by using the number of successful, failed, and canceled projects divided by the total number of projects.

- Finally, I created the line chart as you can see on the picture.

![PivotTable_and_Chart_Outcomes_vs_Goals](https://user-images.githubusercontent.com/89308251/131071975-ddb9f02d-5b92-4ebd-941b-6220f236c133.png)


### 3. Challenges and Difficulties Encountered

   - I had two challenges in this assignment. 
        - The first challenge was placing the appropriate pivot table fields in the columns, rows, and values boxes. I had to experiment with different combinations before I got the right one.
        - The second challenge for me was using the COUNTIFS() functions. After having some difficulties, I realized I had to use the $ before dragging some formulas down. I also realized I had to change the ranges based on their goal amounts.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

    > The two conclusions I can draw from the Theater Outcomes are that the summer months (May to July) tend to be the most successful while the end of the year (December) tends to only succeed about 50% of the time. This might be because people don’t want to spend much money during the Winter holidays.

- What can you conclude about the Outcomes based on Goals?
    
    > I can conclude that fundraisers with lower goals tend to succeed while fundraisers with higher goals tend to fail. However, there are some exceptions which might be explainable by the thinness of the data at those points.

- What are some limitations of this dataset?
    
    > One limitation might be that due to the small sample size, the fundraisers are heavily biased towards fundraisers in the U.S. ¾ of the recorded fundraisers are in the U.S. Also all the fundraisers occurred between 2009 and 2017. It would be helpful to have more recent data. 2017 is already 4 years ago.

- What are some other possible tables and/or graphs that we could create?
    
    > The data that I would want to see would be a table and graph of length of time (in days) compared with outcome of each fundraiser. I could also make a box and whisker plot of the goal and pledged values to see if there is anything interesting to learn from the means and quartiles.




