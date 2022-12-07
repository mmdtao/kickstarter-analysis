# Kickstarting with Excel

## Overview of Project
Louise, an up-and-coming playwright, is looking to crowdfund for her play, "Fever." She wanted previous crowdfunding campaigns analyzed so that she can plan a successful campaign.
### Purpose
Specifically, Louise wants to know how crowdfunding campaigns for plays fared based on the launch date of the campaign as well as based on the funding goals. This will help her determine the right time and amount to start her crowdfunding campaign for "Fever."
## Analysis and Challenges
To determine the right launch date, a pivot table comparing launch date with campaign outcomes was created to be able to sort the "Kickstarter" data to count the "theater" outcomes. Then a line graph was created to visually show the outcomes
### Analysis of Outcomes Based on Launch Date
To create the pivot table, "Parent Category" and "Years" were set as the filters, "outcomes" placed in the columns, "Date Created Conversion" set for rows, and a "Count of outcomes" for the values pulled from the "Kickstarter" sheet. A line graph was then inserted to visualize this data showing months on the x-axis and outcomes on the y-axis. 
Theater_Outcomes_vs_Launch.png
### Analysis of Outcomes Based on Goals
To get a more in-depth perspective of how campaign goals impacted the outcome of those campaigns, the goals were first organized into $5,000 groups. Then the data needed to be organized by its outcomes: successful, failed, and canceled. To pull these values from the "Kickstarter" table, each cell needed to use COUNTIFS equations. My COUNTIFS equations first set the minimum boundary of the goal, followed by the maximum boundary, the outcome string, and lastly the subcategory, "plays" (formula shown below). To crosscheck my table, I matched the sum of "Number Successful" column with the "Subcategory Statistics" sheet. The "Total Projects" column was determined by summing the previous outcome counts. Lastly, the percentages were determined taking the specific outcome count and dividing it by the total for each goal category. These results were then reformatted to show whole percentages. Then a line graph was created placing "Goals" on the x-axis and each percentage column in the y-axis.
Outcomes_vs_Goals.png
### Challenges and Difficulties Encountered
