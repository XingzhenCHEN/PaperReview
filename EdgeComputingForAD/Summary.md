# Edge Computing for Autonomous Driving: Opportunities and Challenges 55



>Vol. 107, No. 8, August 2019 | PROCEEDINGS OF THE IEEE

>SHAOSHAN LIU

# Contribution

## Algorithm Subsystem

**Sensing**: LiDAR Camera Radar and Sonar

**Perception-Localization**: 

**Perception—Object Recognition and Tracking**:A general CNN
evaluation pipeline usually consists of the following layers:
1 the convolution layer uses different filters to extract
different features from the input image. Each filter contains a set of “learnable” parameters that will be derived
after the training stage; 2) the activation layer decides
whether to activate the target neuron; 3) the pooling layer
reduces the spatial size of the representation to reduce the
number of parameters and consequently the computation
in the network; and last, 4) the fully connected layer
connects all neurons to all activations in the previous
layer

object tracking

**Decision** :In the decision stage, action prediction,
path planning, and obstacle avoidance mechanisms are
combined to generate an effective action plan in real time.

One approach would be to use deterministic,
complete algorithms to search all possible paths and utilize
a cost function to identify the best path.

Since safety is of paramount concern in autonomous
driving, we should employ at least two levels of obstacle avoidance mechanisms to ensure that the vehicle will not collide with obstacles.

## Vehicular Edge Subsystem

The vehicular edge subsystem integrates the abovementioned algorithms together to meet real-time and
reliability requirements.

1)the system needs to make sure that the
processing pipeline is fast enough to consume the enormous amount of sensor data generated; 2) if a part of
the system fails, it needs to be robust enough to recover
from the failure; and 3) the system needs to perform all
the computations under energy and resource constraints.

**Hardware Arc**: Nvidia PX platform // TI TDA // Altera Cyclone // Zynq MPSoC //  MobilEye EyeQ5

**Real-Time Operating Systems**:A real-time operating
system (RTOS) is a special operating system intended to
serve real-time applications, such as industrial, automotive, aviation, military, and so on

QNX // VxWorks

**Middleware**:On top of the RTOS, we need a middleware layer to bind different autonomous driving services together.

**ROS**:The first one is reliability; ROS has
a single master and no monitor to recover failed nodes.

Performance is second; when sending out broadcast messages, it duplicates the message multiple times, leading to
performance degradation.

## Cloud sunsystem
The two main
functions provided by the cloud include distributed computing and distributed storage.

**Simulator**

**HD Map Generation** Pose estimation // Data fusion // Three-Dimensional Object Location Detection // Semantics/Attribute Extraction

**Model Training** 

## Benchmarks Tools

data sets and workload

**KITTI** image+LiDAR  //
**TUM RGBD** for SLAM//
**PASCAL3D** 3D object detection//
**MOTChallenge** multi target tracking//



# Reflection
S. Liu, J. Tang, Z. Zhang, and J.-L. Gaudiot,
“Computer architectures for autonomous driving,”
Computer, vol. 50, no. 8, pp. 18–25, 2017.

S.-C. Lin et al., “The architectural implications of
autonomous driving: Constraints and
acceleration,” in Proc. 23rd Int. Conf. Architectural
Support Program. Lang. Oper. Syst., 2018,
pp. 751–766.

J. Tang, B. Yu, S. Liu, Z. Zhang, W. Fang, and
Y. Zhang, “π-SOC heterogeneous SOC
architecture for visual inertial SLAM applications,”
in Proc. IEEE/RSJ Int. Conf. Intell. Robots Syst.
(IROS), Oct. 2018, pp. 1–6.

