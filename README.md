# Bellabeat Case Study

<!-- Background -->
## Background

Urška Sršen and Sando Mur founded Bellabeat, a high-tech company that manufactures health-focused smart products. Bellabeat empowers woman with beautifully designed technology that collects data on activity, sleep, stress, and reproductive health. Bellabeats is a rapidly and quickly growing company, it has many products such as:
 Bellabeat app-provides health data related to their activity, sleep, stress, menstrual cycle, and mindfulness 
Leaf- Bellabeat’s Classic Wellness tracker can be worn as a bracelet, necklace, or clip. Connects to Bellabeat app to track activity, sleep and stress. 
Time- Wellness watch combines the timeless look of a classic timepiece with smart technology to track user activity, sleep and stress. 
Spring- This is a water bottle that tracks daily water intake using smart technology to ensure that you are appropriately hydrated throughout the day. The Spring water bottle connects to the Bellabeat app to track your hydration levels.
I will be focusing on one of the Bellabeat’s products the Leaf and will be analyzing smart device data to gain insight into how consumers are using their smart devices. 


<!-- ASK -->
## ASK

### Business Task

I will be analyzing non-Bellabeat smart device data usage to gain insight into how consumers use non-Bellabeat smart devices. Bellabeat can benefit from learning the trends of smart device usage and determine marketing strategy for the future. 

### Stakeholders
 
  •	Urška Sršen- Bellabeat’s cofounder and Chief Creative Officer

  •	Sando Mur- Bellabeat’s cofounder; Key member of the Bellabeat Executive team 

### Secondary Stakeholders
   •	Bellabeat Marketing Annalytic Team
   
<!-- Prepare -->
## Prepare

•Data Used Fitbit Fitness Tracker data (CC0: public Domain, dataset made available through Mobius) Kaggle Data set
•Data is organized in 18 files in a .CSV format separated by activity, steps and heart rate. 
• Data is a mix of long and wide formats
•The data contains thirty eligible Fitbit users that consented to the submission of personal tracker data, including minute-level and daily activity, steps, and heart rate.

### ROCCC

  •Reliability – Dataset was only collected from 30 individuals and the gender was unknown 
  
  •Originality- Collected from Third party Amazon 
  
  •Comprehensive: Data set contains multiple fields on daily 
  
  •Current- The data set was collected from 3.12.2016-5.12.2016
  
  •Cited- Data collector and source is documented

I will be working with the files: DailyActigity_merged, Dailycalories_merged, dailyintensities_merged, dailysteps_merged, sleepday_merged, weightloginfor_merged. 

<!-- PROCESS -->
## PROCESS
 I will be using Excel Spreadsheets, SQL, and Tableau 
 
 
 ### Cleaning data steps
    •Started opening the files in Excel
    •I noticed that the file DailyActivity has the calories, intensities, and steps all merged in to one. 
    •I removed duplicate, only sheet that needed duplicates removed was sleep merge it went from 2070 to 2055 rows
    •Sepreated date/time column 
    •Uploaded the clean datasets in to SQL


 In SQL I checked for how many participants we had in each dataset 

    SELECT COUNT(DISTINCT Id) AS Total_IDs
     FROM `fitbit_data.Daily_Activity`
    
    Daily_Activity-33
    weight_log- 8
    Sleep_day- 24
    
 Decided not to use the weight_log data since there were few d
 
Starting with Sleep_Day 
SELECT TotalMinutesAsleep/60.0 AS hours FROM `fitbit_data.sleep_day`

<!-- ANALYZE -->
## ANALYZE


<!-- SHARE -->
## SHARE


<!-- ACT -->
## ACT
