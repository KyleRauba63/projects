---
title: "Cyclistic Case Study"
author: "Kyle Rauba"
date: "3/2/2021"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

### The objective of the following case study was to analyze rider data from Cyclistic, a fake bike-rental company, over the timespan of April 2020 - April 2021. Cyclistic has 2 tiers of users: casual riders and annual members. Customers have the option of riding classic, docked or electric bikes. The purpose of the following investigation was to answer the question:

### **How do annual members and casual riders use Cyclistic bikes differently?**

In order to answer this question, data was retrieved from the company's <a href="https://divvy-tripdata.s3.amazonaws.com/index.html">database</a> and the files were unzipped. The data was then cleaned via the creation of uniform column titles, removal of white space and spreadsheets to consolidate quarterly data in. Following cleaning of each data set, the data was manipulated using MS Excel to produce 3 sets of data to answer the above question. 

#### 1. Ride Number
Monthly ride numbers were calculated and compared between casual riders and members. Data manipulation techniques included formatting the data as a table, using the AVERAGE, AVERAGEIF and COUNTA functions and creating new sheets to isolate excluded data with consistent column and sheet labeling conventions.

####### **Figure 1: Unique Ride Numbers. Members had more unique rides than casual riders. Rides peaked in the summer and troughed in the winter.**

![Unique Ride Numbers](https://www.kapwing.com/e/622009cd247184005936db6c) <div style="height: 0; padding-bottom: calc(61.83%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="80%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/622009cd247184005936db6c" style="border:5; height:80%; left:0; overflow:hidden; position:absolute; top:0; width:80%" title="Embedded content made on Kapwing" width="650%"></iframe></div></a></p>
#### 2. Average Ride Time
Ride times were averaged, and compared between unique casual rides and unique member rides. An overall average was calculated for the purpose of comparison.


####### **Figure 2: Average Ride Times. Casual riders tended to ride for longer than members.**
<div style="height: 0; padding-bottom: calc(61.83%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="80%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/621e6ae344a038007fce899b" style="border:5; height:80%; left:0; overflow:hidden; position:absolute; top:0; width:80%" title="Embedded content made on Kapwing" width="65%"></iframe></div></a></p>
#### 3. Preferred Bike Type
Customers have 3 choices of bikes to ride: Classic, Electric and Docked. Customer data was analyzed to compare which bike types casual riders and members preferred.

####### **Figure 3: Member Bike Preference. Members preferred docked bikes overall.**
<div style="height: 0; padding-bottom: calc(28.65%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="80%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/62200aac49f8dc0077bf2928" style="border:5; height:80%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div></a></p>


####### **Figure 4: Casual Bike Preference. Casual riders preferred docked bikes overall.**
<div style="height: 0; padding-bottom: calc(28.65%); position:relative; width: 100%;"><iframe allow="autoplay; gyroscope;" allowfullscreen height="80%" referrerpolicy="strict-origin" src="https://www.kapwing.com/e/62200c363b2a6c00ad36b651" style="border:5; height:80%; left:0; overflow:hidden; position:absolute; top:0; width:100%" title="Embedded content made on Kapwing" width="100%"></iframe></div></a></p>

The results were visualized in a variety of different ways to both: a. Demonstrate competence in R, Excel and Tableau; and b. To provide varying visualizations of the results. 

### Problems that arose
Deciding what data to exclude from the analysis. Data containing a ride time of ERROR or 0 seconds were removed from the dataset and moved to an "exclusions" worksheet.

### Analysis of results 

Overall, Cyclistic consistently had more rides from members than non-members from April 2020- April 2021. (Fig. 1) 

Casual Cyclistic riders tended to ride for longer than Cyclistic members. (Fig. 2)

The data suggests that docked bikes were most popular with Cyclistic customers overall, especially from April 2020- November 2020. Classic bikes saw an inflow of use following a drop in use of docked bikes, from December 2020- April 2021, with members again providing the majority of the rides. Electric bikes saw steady but low overall interest, majorly from members between August 2020 and April 2021. (Figs. 3,4)

Overall, the data suggests that casual users tended to ride longer lengths of time than members and overall preferred docked bikes over electric and classic bikes. Members had the same proclivity towards riding docked bikes but tended to ride for shorter times on average.

### **Based on the results, I would recommend Cyclistic:** 

a. Focus on docked bike inventory over electric and classic bikes.
b. Conduct surveys after rides for riders to uncover motives for a difference in ride time. Questions to ask riders should include what factors influenced both: a. Their ride times, and b. Which type of bike they chose to ride. Responses should be separated by Member/Casual status.
c. Focus marketing efforts during the summer months.
