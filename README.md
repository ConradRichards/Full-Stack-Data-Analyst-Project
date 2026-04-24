# Full-Stack-Data-Analyst-Project
Healthcare Revenue Analytics &amp; Operations Diagnostics
### Exceutive Summary: 
The synthetic raw data set that you will see in the "Raw Data Set" File attached to this Repisitoray was created by AI CLAUDE as well as adjusting it to be realisitc for more analysis for a precicse messy data set to clean in SQL including a/b testing in Python after extracting, transforming and loading the csv file from claude into excel for adjustments. Lastly bringing the data to life to showcase findings and what decision can be made to create impact and resolution to bottle neck issues and reduce churn.  

### Business Problem:
A multispecailty group practice family medicine clinic stated that they were having bottleneck issues regarding there revenue dropping in the year of 2025 compared to 2024. Initailly the providers at the clinic thought that that the solution would be to increase the marketing behind the clinic to find more patients to enroll for treatment as it was due to only reciving only 5 new patients for the year of 2025 vs 2024 having at least 200 new patients enrolled but the data and analytics in the EHR system still wasnt adding up to why the revenue decreased so much in the year of 2025. They asked the data analyst to take a look into the data to see what was going on. Patients are also calling into make an appointment as well as scheduling in person after there current visit for a follow up. Lastly the providers spoke about the accounts recivable following outstanding and that they did not have to chase patients down for missing payments since they would pay there follwoing visits. Patients are required to sign a waiver stating they will pay as well as being given a grace period to pay there balance before returning to treatment. With this being inplace there revenue still went down in the year of 2025 compared to 2024. How we will first start the analysis is by asking the 5 W's Why (Why are we cleaning the data), What (What specific tables/columns/rows/column values are causing the bottleneck issues), Who (who is responsible for the data), and lastly When (When did this issue start).

![image)(https://github.com/ConradRichards/Full-Stack-Data-Analyst-Project/blob/13dc6b2bbd8bd9c6d461825a9fee25ee48f9ac6b/2024%20Revenue.png)
![image](https://github.com/ConradRichards/Full-Stack-Data-Analyst-Project/blob/aae6a712668b66911f3892c56b33f98a2ec62797/2025%20Revenue.png)

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
The suggestion that will be made based upon impact due to the metrics and analsyis is to only scheduled patients within a 14 day period due to a high canceletion rate in the year of 2025 for patients having scheduled over 14 days in advance and having to cancel. The next thing is to send reminder text/emails to patients as this is a high reason for the amount of no shows in the year of 2025. Lastly when taking on handicap patients there is a high chance for canceltion due to transportation issues as this was the case in the year of 2025 which can be comapred to the year of 2024 as well but overlooked due to the revenue made in the year of 2024. A solution to this is depening on the appointment type for the patient, a telehealth visit would be ideal to avoid cancelation issues. Byy doing these things it should show actional insights and increase revenue and fix pipeline issues.

Based upon the findings there were a total of 5,002 patients in 2025 inlcuding 5 new patients and in 2024 there were a total of 4,997 patients inlcuding 200 new patients. Of the 5,002 1,554 patients showed up to there appointments 1,999 did not receive a SMS reminder and did not show up, 1,448 patients cancled and were handicap and scheduled over 14 days in advance and only 1 patient canceled but scheduled within the 14 day timeperiod. so 40% were no shows 30% canceled and 30% showed up in the year of 2025.

![image](https://github.com/ConradRichards/Full-Stack-Data-Analyst-Project/blob/db90b3911dedc884139101dcc015b00b017b61a8/Root%20Cause%20Of%20Analysis%20Chart.png)
