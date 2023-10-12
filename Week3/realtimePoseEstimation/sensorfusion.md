# A real-time pose estimation algorithm based on FPGA and sensor fusion

>L´aszl´o Sch¨affer
>
>SISY 2018


## Contribution
### Background
Using sensor
fusion, the information from the sensors and the characteristics
of each sensor can be used together to improve the estimate
and decrease the uncertainty of the measured variables.


### Solution
In this
paper a real-time pose estimation algorithm using sensor fusion of
visual odometry (optical flow), Inertial Measurement Unit (IMU)
and Global Positioning System (GPS) measurements is presented.


### Result
The proposed low-cost architecture processes
one sensor measurement in 1:95s and consumes only
2 Watts, which enables real-time mobile applications. The
presented algorithm was tested in MATLAB and on the FPGA.
The results showed that the FPGA-based implementation is
358 times faster.
