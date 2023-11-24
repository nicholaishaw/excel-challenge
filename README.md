# Crowdfunding Analysis Using Excel

## Background
Crowdfunding platforms like Kickstarter and Indiegogo have been growing in success and popularity since the late 2000s. From independent content creators to famous celebrities, more and more people are using crowdfunding to launch new products and generate buzz, but not every project has found success.

To receive funding, the project must meet or exceed an initial goal, so many organizations dedicate considerable resources looking through old projects in an attempt to discover “the trick” to finding success. A database of 1,000 sample projects will be analyzed to uncover any hidden trends. The database consisted of an excel file that contained information of each project including the ID number, name of the organization, a brief description of the organization ("blurb"), the goal of the organization's project, the amount of money pledged, the country, the category & subcategory of the project (e.g., food, music, technology, music, etc).

## Analysis
The raw crowdfunding excel file was organized and manipulated to reveal trends in crowdfunding projects. 

**Database Organization.** Conditional formatting was applied to the 'outcome' column to easily identify which projects were successful, failed, or canceled. A 'percent funded' column that used a formula to find how much money a campaign made relative to its initial funding goal. Conditional formatting was applied to this new 'percent funded' column to scale with how the project earnings relative to the funding they received. After condition formatting was applied to both columns, the 'category & subcategory' column was split into two columns: 'category' and 'subcategory' for a more percise analysis of each project. For instance, 'music/rock' in the 'category & subcategory' column would be split into 'music' for the category and 'rock' for the subcategory.

**Pivot Tables.** Three pivot tables were created to provide a better breakdown of the data. The first pivot table showed how many campaigns were successful, failed, canceled, or are currently live per category. A stacked-column pivot chart was created to display the amount of campaigns in these categories and could be filtered by country. The second pivot table showed how many campaigns were successful, failed, or canceled, or are currently live per sub-category
