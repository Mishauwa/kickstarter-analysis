
# Kickstarting with Excel

## Overview of Project

A customer named Louise wants to launch her theater play "Fever" with the help of a fundraising campaign. 
The fundraising campaign is close to it's goal and Louise is planning to launch "Fever" soon.

### Purpose

Before the launch Louise requests to have an advanced analysis about competitive fundraising campaigns.
Especially interesting for her are how other campaigns are behaving in relation to their launch dates and funding goals. 

## Analysis and Challenges

To fulfill Louise request there will be 2 technical analysis performed. 

### Analysis of Outcomes Based on Launch Date

The first analysis "Outcomes based on launch date" is giving insights about the outcome of other campaigns in regards of their launch date. 
Interesting for Louise are the successful, failed and canceled campaigns in the theater parent category over every year since the dataset has started. 
The following graph shows on a monthly basis the outcomes of the campaigns. To create the graph a new column Years has to be created in the main Kickstarter dataset. With that information a Pivot table can be created. The Pivottable has to be filtered based on "Parent Category" and "Years". The Rows uses the- date created conversion and the columns the outcomes. The values uses the count of the outcomes. After grouping the Row Label column to show the months of the years you have to filter for Theater and all Years.  

<img width="338" alt="Theater_Outcomes_vs_Launch" src="https://user-images.githubusercontent.com/69826498/186282319-72da226e-183c-42c9-8a95-a7c766d7063e.png">


### Analysis of Outcomes Based on Goals

The second analysis "Outcomes based on goals" is giving insights about the outcome of other campaigns in the theater subcategory plays in regards their financial goal. Interesting for Louise is in which financial goal ranges the most successful, failed or canceled projects are. With that information she can check and define her fundraising goal. 
The following chart shows the percentage of successful, failed and canceled campaigns for defined financial goal ranges. 
You have to create a new sheet with a table and the defined financial goal ranges. After that you can use the COUNTIFS() function to get the outcomes of the campaigns in the subcategory play based on the financial ranges. With the SUM() function you can populate the "Total Projects" Now you are able to calculate the percentage of the outcomes for the goal ranges. For the Pivot chart you have to use the Goal ranges for the rows and outcome percentages as the values. 

<img width="343" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/69826498/186284694-e086226e-f4a5-4e4a-b6b2-d0ad248c1b04.png">

### Challenges and Difficulties Encountered

I tried to create the Outcomes Based on Goal chart directly in the same worksheet as the created table with the input. 
By creating the Pivot table the rows with the goal ranges got sorted differently than in the initial table. The rows couldn't be changed manually. I had to create a new sheet with the Pivot table. After that it was possible to sort the rows manually. 

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
- In general the most campaigns get started in May and June. 
- May is the best month to launch a succesful campaign in the Theater category. 
- The failed campaigns are over the whole year more stable than the successful ones. That shows that independent of the time of the year there is always a risk to fail. 

### What can you conclude about the Outcomes based on Goals?
- In general you can say the smaller the fundraising goal the more successful it is. 
- The higher the fundraising goal the more campaigns are failing. 

### What are some limitations of this dataset?
- The data doesn't show what actually the reasons for the successful or failed campaings are other then the provided columns like (e.g. financial goal, timing)
- The data gets less accurate the higher the fundraising goals are because there are less campaigns in that ranges. 

### What are some other possible tables and/or graphs that we could create?
- The outcomes based on the fundraiser campaign duration in the theather plays subcategory.
- The average donation and backers counts of the successful, failed and canceled plays based on country. 


