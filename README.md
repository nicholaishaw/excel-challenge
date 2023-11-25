# Excel Crowdfunding Analysis

## Background
Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since the late 2000s. From independent content creators to famous celebrities, more and more people are using crowdfunding to launch new products and generate buzz, but not every project has found success.

To receive funding, the organization must meet or exceed an initial goal, so many organizations dedicate considerable resources looking through old projects in an attempt to discover “the trick” to finding success. A database of 1,000 sample projects was provided to uncover any hidden trends. The database consisted of an excel file that contained information of each project including the ID number, name of the organization, a brief description of the organization ("blurb"), the goal of the organization's project, the amount of money pledged, the country, the category & sub-category of the project (e.g., food, music, technology, music, etc).

In this project, we were tasked with organizing the database by splitting values for easier readability and analysis and creating conditional formatting, creating pivot tables and graphs to examine which categories performed better, and calculating descriptive statistics for the successful and failed outcomes.

## Database Organization
We applied conditional formatting to the 'outcome' column to easily identify which projects were successful, failed, canceled, or currently live. We added a 'percent funded' column formula that calculated much money a campaign made relative to its initial funding goal. We also applied conditional formatting to this new 'percent funded' column, and it scaled with the project earnings relative to the funding they received. After condition formatting was applied to both columns, we split the 'category & subcategory' colum into two columns: 'category' and 'subcategory' for a more percise analysis of each project. For instance, 'music/rock' in the 'category & subcategory' column would be split into 'music' for the category and 'rock' for the sub-category. Lastly, we converted the dates in the 'deadline' and 'launched_at' columns from Unix timestamps into excel date format.

  ![image](https://github.com/nicholaishaw/excel-challenge/assets/135463220/37437e39-4fbd-4c8e-8c24-7a9abeeff169)
  **Figure 1.** *Overview of the conditional formatting applied to the 'outcome' and 'percent funded' columns.*

## Pivot Tables
We generated three pivot tables to provide a better breakdown of the data. The first pivot table showed how many campaigns were successful, failed, canceled, or are currently live per **category**. We added filters so the pivot table can be filtered by country. To visualize the category data, we created a stacked-column pivot chart to display the amount of campaigns were successful, failed, canceled, or are currently live in each category.

The second pivot table showed how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**. We added filters so the pivot table can be filtered by country and primary category. To visualize the sub-category data, we designed a stacked-column pivot chart to display the amount of campaigns were successful, failed, canceled, or are currently live in these sub-categories.

We produced a final pivot table to display information on the number of campaigns that were successful, failed, canceled, or are currently live per month. We added filters so that the pivot table can be filtered based on category and year. We created a pivot-chart line graph to visualize the data.

  ![image](https://github.com/nicholaishaw/excel-challenge/assets/135463220/c3473009-39e8-448f-bdc1-9fdad97521e3)
  **Figure 2.** *A sample pivot table and chart: outcome data per month.*

## Goal Analysis
We created a breakdown of both the amount and percentage of the successful, failed, and canceled projects per funding goal. We added a line graph to illustrate the relationship between relationship between the percent of successful projects and the funding goal.

  ![image](https://github.com/nicholaishaw/excel-challenge/assets/135463220/d144268e-2b00-4791-bc11-f811adba1c04)
  **Figure 3.** *Breakdown of the project outcomes per funding goal.*

## Statistical Analysis
Using VLOOKUP, we returned the number of backers for each project in the successful and unsuccessful outcomes. Using excel formulas, we calculated the mean, median, minimum, and maximum backers and the variance and standard deviations for each outcome.

  ![image](https://github.com/nicholaishaw/excel-challenge/assets/135463220/ef27f623-e166-43e4-bf8d-2b04d4e13bd1)
  **Figure 4.** *Descriptive statistics of the successful and failed outcomes.*

## Final Analysis
Using the pivot tables, graphs, and statistical analysis, it is clear that the highest amount of successful crowdfunding projects were theater projects; however, a closer look at the data reveal that technology possessed the highest rate of success. Not only did tech produce the highest rate of success, it also produced the most amount of money. Within tech, the most successful sub-category was 'web' with a success rate of 70.59%. Audio was excluded from analyses since it only had a sample size of three. A careful look at the monthly outcomes data reveal that the most successful month to start a crowdfunding project is July with a total of 58 successful projects. Since the statistical analysis revealed a high degree of variance within the amount of backers for each outcome, the median best summarizes the data. The data reveal that there is more variance in successful campaigns.
