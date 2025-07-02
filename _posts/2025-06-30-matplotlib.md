---
title: "matplotlib Fun"
date: 2025-06-30 12:00:00 +0000
categories: [matplotlib, python]
tags: [python]
---

Our partner company asked ***How much does down time cost us***

***you can skip this nonsense***  
The whole site is only brought down during severe catastrophes, sundays, and worst of all holidays. No on agrees on what Down-time is but this question did come up while management was negotiating maintenance. Anyways I'm assuming *downtime is the accumulated time machines are inoperable.*
### **Comparing production rates to down time**

One machine going down is drowned out by larger factors like operator performance and teams size so its difficult to measure real impact when multiple things can influence moving the same case/box.

We decided to graph the total summed down time of all machines/conveyors for a period and see if there was a visible impact on warehouse pick rate. Python and matplotlib were fantastic for visualizing this quickly when Excel became complicated.

At an hourly sample production down times were positively correlated because no production means nothing breaking. Moving to a daily period showed the negative correlation we expected.

![rates_image](/assets/img/posts/matplotlib/matplotlib_rate.PNG)

At first the correlation was weaker. Drawing pickrate/downtime points with different colors to see if a factor grouped together based on color and that really helped eliminate some bad data (ie. At 10am everyone in one area goes on break for some reason, saturdays are super light.)

![scatter_image](/assets/img/posts/matplotlib/matplotlib_scatter.PNG)

The scatter plot is missing some context but from it we conclude a total downtime of 5 min per hour seemed to decrease pick rate around 500. Knowing that is nice if you are trying to decide on hiring another operator or maintenance guy.

I love graphs and pretty pictures. You are lucky there are 2 graphs and not 20