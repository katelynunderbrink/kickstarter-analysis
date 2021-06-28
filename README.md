
# kickstarter-analysis
Performing Analysis on Kickstarter data to uncover trends
# Kickstarting with Excel

## Overview of Project

This project was designed to help the client, Louise, determine how different campaigns faired in relation to their launch dates and their funding goals.  

### Purpose

For deliverable 1 was created to visualize the relationship between outcomes and launch month. Deliverable 2 was created to visualize the relationship between the goal amount needed for the campaign and if the campaign was a success or a failure.

## Analysis and Challenges

Deliverable 1 - How I performed analysis
I first created a pivot table in a new worksheet and I filtered the pivot table based off of "parent category" and "years" so I could easily drill down to the information that I need. I then placed Outcomes in the column section, date created in the rows section and count of outcomes in the values section. I had to delete years from the rows section to get it to display by month. I then used the filters I created to drill down to just analyze theater. I then created a line graph based off the data to visualize the outcomes based on launch date. 

Deliverable 2 - How I performed analysis
Deliverable 2 was a little more complicated. I first created a new spreadsheet and populated it with the fields I wanted to analyze. I used the "counties" function to populate my columns. I had to nest code within each other to make sure I was filtering for the measures that I wanted. For example, in cell B2 I wanted to place the number of successful campaigns that were less than 1000. To nest the code I had to make sure that the count ifs applied to the kickstarter tab, and filtered for successful campaigns in column F, campaigns that were under or equal to 1000 in column D and filter for plays in column R. The code ended up looking something like this: =COUNTIFS(Kickstarter!$F:$F,"Successful",Kickstarter!$D:$D,"<=1000",Kickstarter!$R:$R,"plays") I then applied this code to the other columns but changed the goal range and outcomes as it pertained to each column. Once I had all this information filled in, I had to create a line graph to show a the percentage of success as the goal range amounts changed. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85354946/123573693-07261500-d794-11eb-8c90-b829e9c85fe8.png)
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85354946/123573749-1c02a880-d794-11eb-832b-23ad0b5e2f97.png)

### Analysis of Outcomes Based on Launch Date
Successful campaigns were more likely to happen in  the summer months, especially May and were less successful towards the winter months. 

### Analysis of Outcomes Based on Goals
Succesful campaigns did not seem  to correspond too much with funding amount with the exception of the higher numbers being less successful. 

### Challenges and Difficulties Encountered

Deliverable 1 - Challenges 
The only challenge I experienced in this was determining where each variable goes when created a pivot table.

Deliverable 2- Challenges
The biggest challenge I experienced in this was double and triple checking my code to make sure that I had all the formulas properly written out. I realized that I was only using the > sign without using the = sign in the formula so it resulted in many data points being left out. 

## Results

- What are some limitations of this dataset?
In the outcomes based on launch date, there were not a lot of cases to base the analysis on. The way the funding amount categores were grouped led to very few cases per category so it may not be an accurate analysis. 

- What are some other possible tables and/or graphs that we could create?
We could look at countries that did better with plays and we could compare the amount of backers to how much the plays earned. 
