---
title: "matplotlib Fun"
date: 2025-06-30 12:00:00 +0000
categories: [matplotlib, python]
tags: [python]
---

Our partner company asked ***How much does down time cost us?***

### **Comparing production rates to down time**

We wanted to see if more maintanence workers would increase (production) pick rate.

We graphed the total down time of all machines/conveyors for a period to see if there was a visible impact.

It's interesting how equipment not breaking down can correlate with lulls in production.
We actually see lots of downtime during productive periods.
"If you use it, it breaks more." - maintance team
"Cut maintanence and production will skyrocket!" - managment

There's other factors influencing production rate like our operators, stock availability, demand, and equipment redundancy.

Here's a graph!!! It shows a our daily pick rate for 30+ days on top and our accumulated machine downtime at the bottom.
Can you see a negative correalation between the lines?
 
In this picture machine faults lasting longer than an hour are added into the red line and those lasting less than 5 min to the green line
With squinting we can see that long lasting faults are generally more impactfull than a few shorter faults of the same total duration.

![rates_image](/assets/img/posts/matplotlib/matplotlib_rate.PNG)

squint alternative - We can also plot the corelation and color seperate factors. Factor clustered together off the line might suggest something interesting.
Not sure what this graph was but just for an idea

![scatter_image](/assets/img/posts/matplotlib/matplotlib_scatter.PNG)

