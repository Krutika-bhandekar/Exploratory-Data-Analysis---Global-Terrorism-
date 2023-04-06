# Exploratory-Data-Analysis---Global-Terrorism-
# About 
Terrorism is one of the biggest global challenges faced by humanity, killing and wounding millions of people, and responsible for the long-term destruction of wealth opportunities and the well-being of people. Our project is an attempt to dig deep into data to find out the possible ways to prevent terror attacks, initiatives that can be taken for the short and long term for tackling global terrorism, and changing trends in terror attacks to effectively plan mitigation measures for the future.
# Objective
By the end we will conclude the study with following Insights:-

* Which countries were most attacked?
* Which regions were affected the most?
* Is there an increase or decrease in recent years?
* Is there an increase or decrease in the number of successful terror operations?
* Who are the most targeted globally and regionally?
* What are the most common types of attacks globally and regionally?
* What are the most used weapon types globally and regionally?
* Which terrorist organization is responsible for the majority number of attacks? By analyzing these questions, the end goal is to come up with short-term and long-term solutions to stop and tackle terrorism.
# Workflow
1. Understanding problem statement and Raw data
2. Data wrangling: cleaning, manupulation
3. Exploratory Data Analysis
4. Data Visualization
5. Analysing and sharing the conclusions
# 1. Understanding problem statement and Raw data
Firstly very carefully We understand the problem statement and the questions for which we are doing this study. what we want to find out or can find out from the given data set. then we collect data, import it into the system/software. Here we are using "Colab" for this study. Import libraries such as NumPy, pandas, matplotlib, seaborn.Then load the raw dataset. We read the data and try understand the minute detail like what information each column giving and how usefull it can be for the study. we found out that there are 135 variables/Columns with around 1,81,691 entries/Rows. There were few columns which we felt very important to base our study on i.e. Year, Region , Country, State/provs, City, Target type, Attack type etc.
# 2. Data wrangling
Process of cleaning, organizing, and transforming raw data into the desired format for analysts to use for prompt decision-making. Here start finding in the data i.e. Null values, missing values, NaNs, redundant values of data.

a. Handling Null Values
Around 106 columns out of 135 columns were having more than 85% null values, by rule of thumb we have dropped those columns since we cant make better insights out of them. We left with 47 columns after dropping.

b. Dropping unnecessary columns
The columns with the completely numeric representation i.e, nominal data of textual data available in other columns representing the same fact/data were dropped. The dropped columns are as follows country, region, attacktype1, targtype1, targsubtype1,weaptype1, weapsubtype1, natlty1. Also the columns deemed unnecessary for our analysis were dropped. Those columns are guncertain1, individual, dbsource, INT_LOG, INT_IDEO, INT_MISC, INT_ANY, specificity, vicinity, crit1, crit2, crit3, eventid, property, weapsubtype1_txt, targsubtype1_txt, doubter, iday, eventid, extended, target1.

c. Data Manipulation: - Creating new variable/columns by combining other two columns for an effective study i.e.
Victims = No. of Killed + No. of Wounded
