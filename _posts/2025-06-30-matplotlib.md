---
title: "matplotlib Fun"
date: 2025-06-30 12:00:00 +0000
categories: [matplotlib, python]
tags: [python]
---

Our partner company asked ***How much does down time cost us?***

### **Comparing production rates to down time**

Multiple factors influence production (pick rate). There is operator performance, machine redundancy & performance, stock availability, and demand. At the time we wanted to see if more maintanence workers would increase pick rate.

We graphed the total down time of all machines/conveyors for a period and see if there was a visible impact on warehouse pick rate. Python and matplotlib were fantastic for visualizing this quickly where Excel was becoming difficult.

It's interesting how equipment not breaking down can correlate with lulls in production and we see lots of downtime during productive periods.
"If you use it, it breaks more." - maintance team
"Cut our maintanence and production will skyrocket!" - managment

Those other factors like operator presence/performance, stock availability, demand, and redundancy all need to be accounted for in order to see the relationship we want to measure.

Here's a graph!!! It shows a our daily pick rate for 30+ days on top and our accumulated machine downtime at the bottom. Can you see a negative correalation between the lines?

At first the correlation was weaker or non existant. The line colors help identify unexpected factors. 
In this picture machine faults lasting longer than an hour are added into the red line and those lasting less than 5 min to the green li
We can see, with squinting, that long lasting fautls are generally more impactfull than a few shorter faults of the same total duration.

![rates_image](/assets/img/posts/matplotlib/matplotlib_rate.PNG)

squint alternative - Plot the correlation and color the seperate factors.
I should have used a different picture with a factor that shows correlation before and after identifying some factor
I'm not sure but I think this one represents daily periods colored by day of the week?

![scatter_image](/assets/img/posts/matplotlib/matplotlib_scatter.PNG)

The top graph fault points are clickable, and a table is generated showing the faults that were responsible for the point.
If something seems to hugely imact we can identify the culprit machine and fault and take it more seriously the next time.
