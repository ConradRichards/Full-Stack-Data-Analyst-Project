# Full-Stack-Data-Analyst-Project
Healthcare Revenue Analytics &amp; Operations Diagnostics
### Exceutive Summary: 
They stated the problem is _____.   And they also have seen high no show patient appointment rate as well in the EHR system when rescheduling and booking patients. Asking teh 5 W's Why (Why are we cleaning the data), What (What specific tables/columns/rows/column values are cause the bottleneck issue), Who (who is responsible for the data), and lastly When (When did this issue start). The synhtetic data was pulled from AI CLAUDE and Manually Adjusted in excel for a preceise Messy data set to clean in SQL.

### the duplication sql dwh sql is what leads into the null values sql. deleteing duplcaite ppl to then filling in the correct nullvalues i guess  not really

### Methodology: 
1. ELT inclduing Data WareHousing Cleaning inlcuding standardizing data types Once Loaded teh data is extracted and loaded to transformed from excel Into BigQuery to then cleaning out duplicate patient records as well as missing values in BigQuery.
2. Advance Exploratory Data Analysis to see were teh decrease in revenue is coming that is causing the bottle neck issues. This invovled Segmentation Analysis as well as Vadlidate Via Analyis between ___ .which provides insights into user segmentation, behavior patterns, and underperforming areas.
3. Doing an segment by demension analysis in BigQuery to analyze the relationship between on the amount of no shows compared the amount of SMS or Email Reminders sent out or not sent out. Using Contengecy table (cross-tabulation)/conditional count to segment the data.
4. Implenting a validate via sequence anlaysis To validate appointments scheduled exactly or more than 14 days in advance since the optimal booking window is between 0-2 weeks and anything after that can generate cancelation due to forgetting the appointment time or scheduling conflicts.
5. Doing an segment by demension analysis in BigQuery to analyze the relationship between on the amount of handicap patients compared the amount of canceled appointments by handicap patients.
6. Do A/b testing specifically Stastical Significance and creating a null hypothesis and alternative hypothesis as well as contigency tables and stastical testing such a Chi Square Test and T-Test To confirm findings to determine if the differences between groups are statistically significant.  focuses on translating these findings into a rigorous, actionable experiment.
7. Data Visulation to Show Case the findings

### Skills & Systems/Tools Used:
Big Query: SQL, Debugging (syntax corrections, code revewing)

Google Collabatory: Python, Debugging (syntax corrections, code revewing)

Tableau: Data Vizulation Tools Tableau 

### Results & Business Recommendation:
by doing this it should show actional insights and increase in revenue and fix pipeline issues.
