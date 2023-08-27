# Perception Processing Rate Estimation for Safety in Autonomous Vehicles

>DAC 22
>
>main author: Yu-Shun Hsiao

RoboRun employs a model to dynamically adjust accuracy and speed of algorithms based on object density for drones. 

Zhuyi considers more factors (such as actor states and dynamics) and is applied to AVs.

## Contribution
This paper proposes a sensor frame processing rate (FPR) estimation model, Zhuyi, that quantifies the minimum safe FPR continuously in a driving scenario.

### Background

FRP: frame processing rate

1.WE need to ensure the FRP for security

2.We need to adjust the camera calculate recourse when the hardware resource is not available to operate all the data.



### Solution

The Zhuyi model employs kinematics-based calculations to estimate the processing latency requirement per actor and aggregates the requirements based on the cameras’ field of view to obtain the FPR.

Set up a series formula to increase the efficiency of the iteration, which is used to find the best choice.

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/Zhuyi/formula1.png "")


So far, it has estimated the tolerable latency for each actor assuming a single future trajectory.

And to find the FPR per sensor, just reciprocal.
![](https://github.com/XingzhenCHEN/PaperReview/edit/main/Week1/Zhuyi/reciprocal.png "")



### Result

Zhuyi’s estimated FPRs are conservative, yet the system can maintain safety by processing only 36% or fewer frames compared to a default 30-FPR system in the tested scenarios.

And it can be used for:

Post-Deployment: **Work Prioritization**.

Pre-Deployment:xxx

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/Zhuyi/figure3.png "")



## Question







## Reflection




