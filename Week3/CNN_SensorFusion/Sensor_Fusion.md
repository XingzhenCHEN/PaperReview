# Enabling Efficient Deep Convolutional Neural Network-based Sensor Fusion for Autonomous Driving
>Xiaoming Zeng
>
>DAC 22

## Contribution

### Background
However, existing mainstream DCNN fusion strategies conduct
fusion by simply element-wisely adding feature maps extracted
from different modalities together at various stages, failing to
consider whether the features being fused are matched or not.

The middle fusion method with element-wise
summation is the dominant method in recent works
as we can notice in the KITTI benchmarks.

we frustratedly
observe that existing solutions all fail to consider the intrinsic
relationship between two sets of feature maps to be fused.



### Solution
We first propose a feature disparity metric to quantitatively
measure the degree of feature disparity between the fusing
feature maps.

We propose a Fusion-filter as the Featurematching
techniques to tackle the feature-mismatching issue.

A. Feature-matching Utilizing Fusion-Filter



### Result
With the assistance of feature
disparity working as an additional loss, our proposed technologies
enable DCNN to learn corresponding feature maps with similar
characteristics and complementary visual context from different
modalities.

## Reflection
In addition, we learn that high-level feature
maps tend to hold similar features, offering an opportunity
to share the feature-extracting filters residing in deep layers
between two network branches.
