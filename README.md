# slam-learn
>小白slam入门，记录学习过程，如有不正确，欢迎指出！


* [语义分割](#语义分割)
* [动态环境](#动态环境)
* [点、线、面特征建图](#点、线、面特征建图)
* [视觉里程计优化](#视觉里程计优化)
* [后端优化](#后端优化)
* [回环检测](#回环检测)
* [不知道怎么分类](#不知道怎么分类)
* [阅读文献](#阅读文献)

## 语义分割
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   语义定位建图 2、3、8、10； Visual Mapping 3；全局定位 5

-RoadMap: A Light-Weight Semantic Map for Visual Localization towards Autonomous Driving

-Road Mapping and Localization Using Sparse Semantic Visual Features

-Robust Semantic Map Matching Algorithm Based on Probabilistic Registration Model

-Robust Improvement in 3D Object Landmark Inference for Semantic Mapping

-Lightweight Semantic Mesh Mapping for Autonomous Vehicles

-**Semantic Histogram Based Graph Matching for Real-Time Multi-Robot Global Localization in Large Scale Environment**

## 动态环境
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   Visual SLAM 13; 后端 2

-DOT: Dynamic Object Tracking for Visual SLAM 

-A Switching-Coupled Backend for Simultaneous Localization and Dynamic Object Tracking


## 点、线、面特征建图
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   Visual SLAM 9; VO 1 ；feature：1；
 
-Avoiding Degeneracy for Monocular Visual SLAM with Point and Line Features

-Accurate and Robust Scale Recovery for Monocular Visual Odometry Based on Plane Geometry

-SKD: Keypoint Detection for Point Clouds Using Saliency Estimation

## 视觉里程计优化
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   VO 5、6、8；VIO 4、8、10、12

-Learning Optical Flow with R-CNN for Visual Odometry

-Optimizing RGB-D Fusion for Accurate 6DoF Pose Estimation

-Continuous Scale-Space Direct Image Alignment for Visual Odometry from RGB-D Images

-Direct Sparse Stereo Visual-Inertial Global Odometry

-Bidirectional Trajectory Computation for Odometer-Aided Visual-Inertial SLAM

-An Equivariant Filter for Visual Inertial Odometry 

-Cooperative Visual-Inertial Odometry


## 后端优化
```  
```  
## 回环检测
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   视觉场景识别 除了6、7；

-Intelligent Reference Curation for Visual Place Recognition Via Bayesian Selective Fusion 

-Appearance-Based Loop Closure Detection Via Bidirectional Manifold Representation Consensus

-SoftMP: Attentive Feature Pooling for Joint Local Feature Detection and Description for Place Recognition in Changing Environments

-Simultaneous Multi-Level Descriptor Learning and Semantic Segmentation for Domain-Specific Relocalization

-Resolving Place Recognition Inconsistencies Using Intra-Set Similarities 

-Spherical Multi-Modal Place Recognition for Heterogeneous Sensor Systems 

-Retrieval and Localization with Observation Constraints

-A Flexible and Efficient Loop Closure Detection Based on Motion Knowledge

-Semantic Reinforced Attention Learning for Visual Place Recognition

-STA-VPR: Spatio-Temporal Alignment for Visual Place Recognition 

-Visual Place Recognition Via Local Affine Preserving Matching

## 不知道怎么分类
>[ICRA 2021](https://blog.csdn.net/xhtchina/article/details/118101298)   Visual SLAM 4,7,8,18

-Multi-Parameter Optimization for a Robust RGB-D SLAM System

-ManhattanSLAM: Robust Planar Tracking and Mapping Leveraging Mixture of Manhattan Frames

-Markov Parallel Tracking and Mapping for Probabilistic SLAM

-VOLDOR-SLAM: For the Times When Feature-Based or Direct Methods Are Not Good Enough

## 阅读文献
>[FSD-SLAM: a fast semi-direct SLAM algorithm](https://link.springer.com/article/10.1007/s40747-021-00323-y)   

针对：复杂环境中由于快速运动和非结构化场景而导致特征丢失；缺乏视觉特征和低纹理环境。
主要思想：将特征点方法与直接方法相结合，
具体工作：
(1)开发了基于子图的特征增强模块，以更稳定地提取图像特征点。
(2)针对摄像机姿态估计问题，提出了一种表观形状加权融合方法，该方法在没有特征点的情况下仍能稳健工作。
(3)研究了一种用于优化相机姿态估计误差的增量动态协方差缩放算法。
(4)基于优化后的相机姿态，设计了人脸元素模型，对点云姿态进行估计和融合，得到理想的三维点云地图。
