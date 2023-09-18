# Neural Pruning Search for Real-Time Object Detection of Autonomous Vehicles

>DAC 21
>
>Pu Zhao NEU


## Contribution
As the first contribution, we generalize the concept of fine-grained structured pruning to cover all types of CONV and FC layers




### Background 

2D and 3D detection makes use of the 2D image and 3D point clouds information from camera and LiDAR sensors, respectively, to detect objects in the environments,

DNN weight pruning has been proved as an effective model compression technique to remove redundant weights, 
Existing work mainly focus on unstructured pruning where arbitrary weight can be removed, 
and (coarse-grained) structured pruning  to eliminate whole filters. 
The former results in high accuracy but limited hardware parallelism (and acceleration),
while the latter is the opposite.

