# Kickstarting with Excel

## Overview of Project
Louise, an up-and-coming playwright, is looking to crowdfund for her play, "Fever." She wanted previous crowdfunding campaigns analyzed so that she can plan a successful campaign.
### Purpose
Specifically, Louise wants to know how crowdfunding campaigns for plays fared based on the launch date of the campaign as well as based on the funding goals. This will help her determine the right time and amount to start her crowdfunding campaign for "Fever."
## Analysis and Challenges
To determine the right launch date, a pivot table comparing launch date with campaign outcomes was created to be able to sort the "Kickstarter" data and count the "theater" outcomes. Once the table was created and filtered to show only "Theater" data, a line graph was created to visualize this data showing months on the x-axis and outcomes on the y-axis. 

To get a more in-depth perspective of how campaign goals impacted the outcome of those campaigns, the goals were first organized into $5,000 groups. Then the data needed to be organized by its outcomes: successful, failed, and canceled. To pull these values from the "Kickstarter" table, each cell needed to use COUNTIF equations. My COUNTIF equations first set the minimum boundary of the goal, followed by the maximum boundary, the outcome string, and lastly the subcategory, "plays" (shown below): 

<img width="592" alt="Kickstarter CountIf code" src="https://user-images.githubusercontent.com/114324871/206075586-03a65ee8-1694-4c21-a632-d89769225379.png">

To crosscheck my table, I matched the sum of "Number Successful" column with the "Subcategory Statistics" sheet. The "Total Projects" column was determined by summing the previous outcome counts. Lastly, the percentages were determined taking the specific outcome count and dividing it by the total for each goal category. These results were then reformatted to show whole percentages. Then a line graph was created placing "Goals" on the x-axis and each percentage column in the y-axis.

While I did not have many difficulties with the COUNTIF statements, I found it tedious and was constantly making sure I had my constraints right for each Goal group. While crosschecking the "Total Projects" in my table compared to the "Subcategory" pivot table, I noticed I was missing a single data point. To correct this, I looked at my COUNTIF code (example above) and had not included a "<=" statement meaning that the single data point fell exactly on one of my constraints.
### Analysis of Outcomes Based on Launch Date
In determining the ideal launch date for Louise's play, the "Theater Outcomes Based on Launch Date" graph (shown below) helps visually show the data filtered by the pivot table. It is clear that the highest percentage of successful campaigns were launched in May with 111 successful campaigns compared to 52 failed campaigns. In general, the best period to launch her campaign should fall between May and July. The graph also shows that December should be avoided since the number of successful campaigns and failed campaigns were nearly the same.
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/114324871/206073006-90197def-7b0e-4e36-9cf9-32a4a0de4507.png)

### Analysis of Outcomes Based on Goals
When analyzing the successful of campaigns based on goal amount, it can be inferred that Louise has a higher chance for a successful campaign with goals under $20,000. From the graph, the campaign goals between $15,000 to $19,999 is an inflection point where larger goals have a higher likeliness of failure. Since her goal is to raise around $4,000, the data showing the campaign goals between $1,000 and $4,999 suggests there is a high likeliness to achieve that goal and more specifically 73% of goals within that range were successful (shown below). 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/114324871/206073002-97ea610a-d148-4f06-bb05-f5ba87f0a296.png)
### Challenges and Difficulties Encountered
While the analysis suggests that Louise should start her crowdfunding campaign for "Fever" should begin in May and that $4,000 is a achievable target, the dataset lacks a correlation between launch date and funding goals. Another table that could be created based on the graphs generated would be to compare campaign success in the months of May, June, and July sorted into the goal amounts. This would give a clearer idea of whether a $4,000 campaign goal would be a achievable target for the month of May if she were to choose that month. The graph I think would be most helpful would show the different fundraising goal ranges on the x-axis and success percentage on the y-axis. 
