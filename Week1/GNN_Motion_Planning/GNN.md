# Hardware Architecture of Graph Neural Network-enabled Motion Planner
>ICCAD 22
>
>Main author:  Lingyi Huang


## Contribution

Compared with uniform sparse matrix multiplication (SpMM)-based solution


### Background

planning solution:1.sampling based RRT/RRT*/PRM 2.graph based. A*

the existing research outcomes cannot be properly
applied to realize efficient GNN-format motion planner because of
the fundamental algorithmic difference

Just focus on the GNN explorer.

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/GNN_Motion_Planning/workflow.png)

the neural path explorers need to process and update feature vector for each edge

BUT the present customized hardware is only deesighed to focus on GCN, which is only involved with processing feature vector of each vertex.!!!


### Solution

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/GNN_Motion_Planning/figure2.png)

SRAM store coresponding infomation.

The main content is the two Engines.

1.Combination Engine:

The combination engine is designed as a
2-D systolic array to support GEMM (general matrix multiplication)


![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/GNN_Motion_Planning/figure3.png)


2.Aggregation Engine.

The aggregation engine aims to accelerate the aggregation phase that is desired in the proposed neural path explorer

is designed as a two-dimension Processing Element (PE) array,

![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/GNN_Motion_Planning/figure4.png)

Also, adjust the order of the reading sequence, to make the workload more balance.


![](https://github.com/XingzhenCHEN/PaperReview/blob/main/Week1/GNN_Motion_Planning/figure5.png)






## Questions (paper links)
1.Chenning Yu and Sicun Gao. 2021. Reducing collision checking for samplingbased
motion planning using graph neural networks. Advances in Neural Information
Processing Systems 34 (2021), 4274–4289.

2.Grapg Theory.


## Reflection
The data flow spend too much time on "on-chip to off-chip memory", maybe we can speed up in this part.



