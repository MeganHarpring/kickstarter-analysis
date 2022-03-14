# **Kickstarting with Excel**

## **Overview of Project**
  Louise's play *Fever* came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals. Using the Kickstarter dataset, I will visualize campaign outcomes based on their launch dates and their funding goals.
  
### **Purpose**
  The purpose of this project is to visualize and analyze what times of year would be the best to start a campaign and what amount (goal) will be the most likely to end with a successful outcome for the fundraiser. 
  
## **Analysis and Challenges**
  I have performed two different analysis to help Louise: Outcomes Based on Launch Dates and Outcomes Based on Goals. These tables and charts will help me to visualize and analyze the right data and trends so that Louise can make an informed decision on her fundraising campaign. I did encounter a few challenges when trying to narrow down the data needed to create the charts but was ultimately successful.
  
 ### **Analysis of Outcomes Based on Launch Date**
  - First, in order to get the correct launch date I had to convert it from UNIX timestamp so that we could see the date in Month/Day/Year form. Then I used the YEAR() formula to get the year from the date.

<img width="177" alt="Date Conversion Formula" src="https://user-images.githubusercontent.com/100392991/158097969-b72d28bc-1363-4e58-80ac-964dd4b87c3d.png">
   
<img width="74" alt="Date Launched" src="https://user-images.githubusercontent.com/100392991/158098054-d2319728-0148-494c-9ede-c90d527adf26.png">

  - Second, I created a Pivot Table with the filters "Parent Category" and "Years", and under "Parent Category" chose only the "theater" category to show up since that is all that Louise was interested in. I also filtered the table to show only the following:
  <img width="171" alt="image" src="https://user-images.githubusercontent.com/100392991/158098665-59e78440-a8dc-4a6f-b015-66abe92bb126.png">
<img width="220" alt="image" src="https://user-images.githubusercontent.com/100392991/158098753-aea63e18-ce2a-45f2-8cee-e97dfc5a152f.png">
  - Thus, creating this Pivot Chart: <img width="218" alt="image" src="https://user-images.githubusercontent.com/100392991/158098988-acab8c89-0069-4da8-8970-a7fa4df1cde7.png">
  - Lastly, seeing as it is hard to visualize the data or see what trends there are, I created this line chart which shows us the relationship between "Successful", "Failed", and "Canceled" campaigns and the months that they were started.[Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/100392991/158099142-bf3ef1e1-670c-468c-8a41-3cab9c9c8921.png)
  
  -This chart helped us to conclude that a campaign launched in May and June have the best chance to succeeding. Also, I would avoiding launching in January as it seems that is when most campaigns were cancelled and there just doesn't seem to be many campaigns going on during that time. 

### **Analysis of Outcomes Based on Goals**
  - First, I created a new excel sheet with with the following column headers and row dollar amounts: 
 <img width="475" alt="image" src="https://user-images.githubusercontent.com/100392991/158099553-a402ee99-6675-4a7c-a83e-1636fd4cde11.png">  <img width="50" alt="image" src="https://user-images.githubusercontent.com/100392991/158099785-1f2999ea-88b8-42b9-8671-a246460b0199.png">
 
  - Second, I used the COUNTIFS formula to fill in the table like so:
<img width="338" alt="image" src="https://user-images.githubusercontent.com/100392991/158099883-f92ba692-ab09-4862-94a9-ab52198b7c3f.png">
<img width="422" alt="image" src="https://user-images.githubusercontent.com/100392991/158099943-cfc54113-ccfd-4adf-9d94-952d8576f944.png">
  - Third, I used the SUM() formula and found the percentages to fill in the rest of the table. 
  - Finally, I inserted a line chart to show the percentage of "Successful", "Failed", and "Canceled" plays by diffeent goal ranges. 
  ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/100392991/158100300-8c4c9853-5d1d-417e-85be-0b09d5d218be.png)
  
  - This chart shows me a couple of different things: I would probably try to keep my goal for funding under 15K, there are quite a bit of successful campaigns in the 35K to 45K range but there is a higher fail rate for those ranges too. 
 

### **Challenges and Difficulties Encountered**
  - The only challenge or difficulty that I encounter was with using the formulas in Excel. The Date Conversion function and the COUNTIFS function took me some time to review and watch videos on. The date conversion was just difficult for me to comprehend how that formula converted the dates, plus I have never heard of UNIX timestamp. Secondly, the COUNTIFS function was just nailing down the greater than, less than, and equal to symbols and where they belong so that I get the correct answer. Also, just learning how to use COUNTIFS, knowing which columns and rows you need to filter to get the correct data that you need was somewhat time consuming but ultimately not too hard to figure out. 

## **Results**

**What are two conclusions you can draw about the Outcomes based on Launch Date?**
  1) The highest number of cancelations for theater is in January.
  2) The highest number of failures is in the summer months but that is also the time range with the most successful campaigns. The ratio of success to failure tells me that even with a high fail rate the success rate is much better, so I would launch sometime between May, June, and July. 

**What can you conclude about the Outcomes based on Goals?**
  1) The higher the funding amount gets the lower the success percent gets and the higher the failure percent gets, thus it would be best to keep your funding goal as low as possible for a better chance at completing your goal. 

**What aee some limitations of this dataset?**
  1) Not having specific location included. The location of these campaigns could make a difference in how much certain campaigns received because the average income could vary quite a bit in different locations, thus, effecting the amount funded. 

**What are some other possible tables and/or graphs that we could create?**
  1) We could create a table and graph that shows the relationship between successful, failed, and canceled campaigns to location or a table and chart to show the relationship between Succcessful Campaigns Goal amount and location. These would both show us how location can effect the funding amount and whether a campaign succeeds or fails. 



