# kickstarter-analysis


## Discovering trends on Kickstarter data


### **Overview**

For this assignment I used Excel to explore Kickstarter data related to arts funding, to help a client determine best practices for a successful theater campaign.

### **Analysis and Challenges**

For my analysis I made two new worksheets based on data from the original Kickstarter data table. 

#### Outcomes vs. Launch Date by Month

For the first worksheet I looked at outcomes by launch date each month over several years, with a focus on theater, as that was most relevant to my client's goals and interests. I used data from successful, failed and canceled kickstarters, and created a pivot table to insert a line chart for clear review of whether a kickstarter was likely to be successful based on the month of the year in which it was held. There were some challenges based on how to best filter the pivot table that were overcome with some quick trial and error to achieve the desired result.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/105175961/198416346-57e84742-2437-450c-909c-18abe25bd312.png)

#### Rate of Success based on Fundraising Goals

For the second worksheet, I created a new table to show kickstarter outcomes based on the goal of the fundraiser in dollar amounts. In increments of $5000 starting at $1000 and going up to $50,000, I tallied the number of successful, failed and canceled campaigns and the percentage of each based on the total number of campaigns in that goal range. To do this I used the COUNTIFS function to find the number of campaigns in that price range, then used the SUM function to determine the percentage of those whether successful or not, based on the results of the COUNTIFS function and the total number of campaigns in that range. Using the COUNTIFS function took some testing and retesting as multiple arguements were needed with clear and concise syntax to pull several data points from the main Kickstarter sheet.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/105175961/198416359-6f54e392-3ac2-4af2-bc69-17f1bf9a87eb.png)

### **Results**

#### Result of Outcomes vs. Launch Date

This line chart shows us that fundraisers that begin in May are by far the most successful, with summer being a more successful time overall. However, looking at failed fundraisers, there are also more fundraisers that fail to meet their goal in the summer than the rest of the year. It may be that more fundraisers are held in the summer overall. Winter seems to be a slow time for kickstarters, with a lower number of successful fundraisers held in December than any other month out of the year.

#### Result of Rate of Success Based on Fundraising Goals

It appears from the graph and data presented that theater productions with fairly low fundraising goals (<$5000 and closer to $1000) were the most successful. Fundraisers with goals less than $1000 had a success rate of 100%. These fundraisers may be more successful simply because they have set such a low fundraising goal, whether that is due to low production costs or not. There is also a jump in the success rate for kickstarters with a fundraising goal in the $35000 to $45000 range. This is based on only 9 kickstarters with a 67% success rate so while not wildly successful, a majority of the fundraisers in this range did meet their goal. 

#### Potential Limitations

While overall this is quite a large dataset to pull information from, I think it would have been helpful to know production costs in relation to fundraising goals. It coud potentially shed some light on why certain productions chose their fundraising goals and whether or not they did so to portray more successful campaigns. It also would have been interesting to view data by year rather than by month when looking at outcomes by launch date or success rate based on goals, to see if there is some ebb and flow to the overall success and popularity of theater from one year to the next.






