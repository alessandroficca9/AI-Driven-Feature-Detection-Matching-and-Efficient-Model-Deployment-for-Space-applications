<div align="center">

# AI-Driven Feature Detection Matching and Efficient Model Deployment for Space Applications  

## Master's Degree Thesis in Data Science and Engineering at Politecnico di Torino, in collaboration with AIKO.

</div>

## Abstract
In computer vision, the Feature Detection and Matching (FDM) task has been widely developed and innovated over the years, achieving the potential to be applied in many use cases. Its primary objective is to extract and establish accurate and reliable feature correspondences between different images, forming the foundations for various applications, including autonomous visual navigation, 3D reconstruction, object detection and tracking. 
This thesis is dedicated to testing and validating FDM algorithms in space-related contexts, focusing on Rendezvous and Proximity Operations (RPO). In this scenario, a chaser spacecraft acquires and processes visual information of a target spacecraft, relying on features matching for localization and navigation.

The objective is to assess local feature detection and matching methods under standard space image conditions, which are characterised by factors such as extreme variations in illumination and limited visual information that can affect reliability and accuracy. The experiments evaluate performance under various circumstances, including significant changes in viewpoint and different object-to-camera distances. They also investigate domain differences by comparing synthetic and real images. Evaluations are conducted on images from the SPEED, SPEED+, and SPEED-UE-Cube datasets.

One of the challenges in FDM is defining reliable evaluation metrics. In space contexts, the absence of suitable datasets and precise ground truth information requires the use of indirect metrics. Based on the detected feature correspondences, these metrics compute secondary information on the geometric relationship between the images. Specifically, the Relative Pose estimation and Homography estimation metrics are considered.
The advent of Machine Learning and Deep Learning has provided the opportunity for significant progress, particularly with the introduction of Transformer architectures that have established a new state-of-the-art approach to computer vision tasks. Accordingly, the study explores classical feature detector and descriptor algorithms such as SIFT, ORB, and AKAZE compared to AI-based models, including SuperPoint, LightGlue, and LoFTR. Experimental results have demonstrated the overall superior performance of DL approaches compared to handcrafted algorithms, particularly in extracting more relevant, repeatable, and robust features.

In the final phase, the thesis investigates the application of the Knowledge Distillation (KD) technique, which has become relevant for the development of efficient and optimized DL models.  Its implementation aims to transfer knowledge from a Transformer-based to a convolutional-based model, motivated by hardware constraints. Hardware space grade currently offers limited support for specific architectural types and operations. Deploying a Transformer-based architecture may be impractical or inefficient compared to more consolidated convolutional layers. In this framework, the work focuses on LigthGlue, which is an AI model specialized in the feature-matching process and operates in conjunction with SuperPoint as a feature extractor.  LightGlue plays the role of the teacher, while the student incorporates modifications in order to replace the Attention-based modules present in the original architecture.

This project conducts preliminary analyses to explore the adaptation and application of these methods, originally developed and tested in general domains, to space-related environments.
