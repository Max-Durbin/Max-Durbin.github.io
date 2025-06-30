---
title: "matplotlib Fun"
date: 2025-06-30 12:00:00 +0000
categories: [matplotlib, python]
tags: [python]
---

During a negation of a maintenance contract someone new but up in our partner company asked *"How much does down time cost us"*. It's a pretty obvious question but none of us knew.

The machines/conveyors are very redundant. The whole site is only brought down during severe catastrophes, sundays, and holidays. One machine going down is drowned out by larger factors like operator performance and teams size. In most cases downtime like this is not detectable. 

We decided to graph the total summed down time of all machines/conveyors for a period and hoped to see an impact on warehouse pick rate. Python was fantastic for doing this quickly, it was also a good excuse to use matplotlib.

At an hourly sample production and down times were positively correlated because no production means nothing breaking. Moving to a daily period showed the negative correlation we expected.

![rates_image](/assets/img/posts/matplotlib/matplotlib_rate.PNG)

At first the correlation was weaker. Drawing pickrate/downtime points with different colors to see if a factor grouped together really helped eliminate some bad data (ie. At 10am everyone in one area goes on break for some reason, saturdays are super light.)

![scatter_image](/assets/img/posts/matplotlib/matplotlib_scatter.PNG)

Anyways from that the total downtime of 5 min per hour seemed to decrease pick rate around 500.