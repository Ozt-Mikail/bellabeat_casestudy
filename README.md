# CASE STUDY: Bellabeat Fitness Data Analysis 
##### Author: Mikail Ö.


##### Date: January 20, 2023


#
The case study follows the six step data analysis process:

### [Ask](#1-ask)
### [Prepare](#2-prepare)
### [Process](#3-process)
### [Analyze](#4-analyze)
### [Share](#5-share)
### [Act](#6-act)

## Scenario
Bellabeat is a successful small manufacturer of health focused products for women. They now have the ambition to become a larger player in the global smart devices market. The Chief Creative Officer, Urška Sršen, wants to gain insights into how consumers are using their smart devices. These insights will help guide the marketing strategy.
 
## 1. Ask

**Problem**: Our Chief Creative Officer needs insights in order to develop an effective strategy with the goal to gain more customers and a bigger market share.   
**Key question**: What are the main trends in smart device usage and how can these trends help influencing Bellabeats marketing strategy?

**Deliverables**:
1. Documentation of the Data Analysis process (this README.md file)
2. Documentation of any cleaning or manipulation of Data (Bellabeat_Casestudy.ipynb file)
3. Data Visualisation with Tableau
4. Summary, key findings and recommendations (Bellabeat_Casestudy.pptx)

**Suggested time frame**: 4-6 hours

## 2. Prepare 
For the anlysis the public Dataset ["FitBit Fitness Tracker Data"](https://www.kaggle.com/datasets/arashnic/fitbit) from Möbius is used. <br>

- The Dataset contains 18 fiels
- Inspection of dataset with Excel (PowerQuery)

Checking if data follows the ROCCC prinzipals:

- reliable: the data was tracked via Fitbit trackers. -> Possible issues with accuracy
- original: Thirty eligible Fitbit users consented to the submission of personal tracker data. The users Möbius published the dataset. ->  No issues with originality 
- comprehensive: includes minute-level output for physical activity, heart rate, and sleep monitoring. -> no issues
- current: The data was collected between 03.12.2016 and 05.12.2016. -> Mostly health related data which does not change over time, assumption that costumer behavior did not change in the last 7 years. 
- cited : Dataset was downloaded around 70 000 times and has a usability score of 100% on Kaggel. -> no Issues

Limitations:


## 3. Process

In this step I check for wrong, missing and duplicate data in the main 5 tables used in this analysis. After this step, I clean and transform the data so it can be used for analysis. See Bellabeat_Casestudy.ipynb file for detailed documentation of this process.

**3.1 checking data integrity**
- To check data integrity we first need to get a quick overview of our data with the str() and head() functions.
- We now check for how many unique users each table has and notice that the tables have different numbers of unique users -> There are 30 participants but activity and calories have 33 different id numbers. Weight has only 8.
- Next, we examine if there are any missing data points -> Table weight has 65 missing data points.
- Lastly, we check if any Tabl has duplicates. -> The daily sleep table has 3 duplicates.
 
**3.2 cleaning process** 

Now it's time to clean the data. First, we delete the duplicates. Then we convert the date column into the time and date format. There is currently no way to restore missing data. So we have to work with the data we have. 

**3.3 tranformation porcess**

For our analysis process we merge the the activity table and the sleep table.

## 4. Analyze


## 5. Share 


## 6. Act
