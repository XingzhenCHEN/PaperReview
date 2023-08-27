# RoboRun: A Robot Runtime to Exploit Spatial Heterogeneity

>Conference: DAC 21
>
>Author:Behzad Boroujerdian


## Contribution
This paper introduces RoboRun, a mobile-robot runtime that dynamically exploits the compute-environment synergy to improve performance and energy. 

Compare with best **spatial oblivious** **static** design.


### Background
a crucial shortcoming of best computing solutions is that they make static, worst-case assumptions about the robot’s operating environment.

Decision latency is the processing time of each sampled input.

Decision deadline is the maximum latency that can be tolerated while ensuring a collision-free flight.

space precision and volume determine the processing latency while space visibility and traversal speed impose the dead- line

![22](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/RoboRun/Figures/fogure1.png "111")



### Solution
identify four different features causing space heterogeneity and quantify their impact on compute

**space precision//space volume//space traversal speed//space visibility**

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/RoboRun/Figures/whole.png)

the governor: calculate the estimatated time budget, and determine the precision and volumn per stage.

the profiler: post-process data to calculate some variables, which is used for Precision Volumn and Deadline.

Operator:

Precision Operator: control the precision of space process (control the sampling distance)

Volumn Operator: 1.control the volume of space added to the map;2.control the space volume communicated to the planner;3.control the space volume explored by the planner



### Result
RoboRun
improves velocity, mission time, and energy consumption by 5X,
4.5X, and 4X. It also reduces CPU utilization by 36% freeing
up computational resources for higher-level cognitive tasks such
as semantic labeling. Our environment sensitivity analysis shows
that RoboRun is more sensitive (1.5X vs. 1.1X) to environment
heterogeneity, indicating its higher environmental awareness. Finally,
RoboRun is better suited for long-distance missions as it is less
sensitive (1.3X vs. 2X) to the distance of the goal location.



## Question
1.Why the green line increases during 30-40s?
![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/RoboRun/Figures/Fig5b.png)






## Reflection

We need OPEN SOURCE!!

We can detect the position and decide the calculation frequency to ddecrease the cost.
