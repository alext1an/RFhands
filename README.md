# RFhands
**Deep Learning-based Hand Gesture Recognition Using Wireless RF Signals**

基于无线射频信号的深度学习手势识别方法

![demo](https://github.com/xiaochouyulalala/RFhands/assets/70216817/5b16442e-9568-4702-95fc-c67e69bcb101)

## Abstract
This study presents RFhands, a novel hand keypoint recognition method that combines wireless radio frequency (RF) signals with deep learning to deliver a privacy-friendly solution that does not rely on visual sensors. The method transmits and receives raw RF signals through an antenna array, applies deep learning to extract meaningful features, and reconstructs hand keypoint data from those features. Experimental results show that RFhands performs well across diverse environments and gestures, achieving high accuracy and robustness. The system demonstrates the potential of RF-based gesture recognition as a privacy-preserving alternative to camera-based approaches, and extends the applicability of wireless sensing technology to a broader range of scenarios.

## 摘要
本研究提出了一种新型的手部关键点识别方法RFhands，利用无线射频信号与深度学习技术相结合，以提供一种不依赖视觉传感器的隐私友好型解决方案。该方法通过射频天线阵列发射和接收原始射频信号，并应用深度学习技术提取有效信息，进一步得到手部关键点的数据。实验结果显示，RFhands在多种实验环境和手势下均表现出色，具有较高的准确性和鲁棒性，展示了其在手势识别中的应用潜力，提供了一种不依赖视觉传感器的隐私友好解决方案，扩展了无线感知技术的应用场景和环境适应性。未来的研究方向包括进一步提升模型的精度和实时性，探索更多应用场景，并改进射频信号的处理技术。

## Background
Gesture interaction is increasingly important in modern human-computer interaction. However, current camera-based gesture recognition systems suffer from privacy risks and sensitivity to lighting and occlusion. RF signal-based detection offers a compelling alternative: it protects user privacy, provides wide sensing coverage, is robust to occlusion and lighting variation, consumes less power, and can serve as an alternative or complementary input modality in mixed-reality devices.

## 背景
手势交互在现代人机交互中至关重要，但当前基于摄像头的手势识别方法存在隐私保护不足和光线遮挡问题。基于无线射频信号的检测方案有助于保护用户隐私，具有广阔的传感范围，抗遮挡和光线变化鲁棒性强且功耗更低，能在混合现实设备中作为替代或补充方案。

## Research Goal
The goal of this research is to combine wireless RF signals with deep learning to propose RFhands, a novel hand keypoint recognition method, and to validate it through comprehensive experiments.

## 研究目标
本研究的目标是利用无线射频信号与深度学习技术相结合，提出一种新型的手部关键点识别方法RFhands，并进行了详尽的实验验证。

## Method
RFhands transmits and receives raw RF signals through an antenna array, then applies preprocessing and deep learning model analysis to construct a 3D hand skeleton model. The overall system architecture is an encoder-decoder structure: an RF signal deep neural network serves as the encoder, and a multi-layer fully connected network serves as the hand keypoint regression decoder.

## 方法
RFhands方法通过射频天线阵列发射和接收原始射频信号，经过预处理和深度学习模型分析构建手部三维骨架模型。系统整体的架构是一个编码器-解码器结构，包括射频信号深度神经网络作为编码器，多层全连接层构建的手部关键点回归网络作为解码器。

![image](https://github.com/xiaochouyulalala/RFhands/assets/70216817/2b106a01-d06b-4e46-a472-f29889b892be)

## Experiments
This study uses a pipeline approach to collect RF and visual data, forming two primary datasets: a VR dataset and a general dataset. The RFhands model is implemented in PyTorch and trained on a cloud server with an NVIDIA RTX 3060 GPU. Model evaluation uses the VR gesture dataset and the general gesture dataset, with Percentage of Correct Keypoints (PCK) and Mean Per Joint Position Error (MPJPE) as the primary metrics.

## 实验
本研究采用了流程化的方法来收集射频和视觉数据，形成了VR数据集和通用数据集两个主要数据集。RFhands模型使用PyTorch实现，并在云服务器上使用NVIDIA RTX3060显卡进行训练。模型评估通过VR手势数据集和通用手势数据集进行，采用正确关键点百分比（PCK）和每个关节位置的平均误差（MPJPE）作为主要评估标准。

![image](https://github.com/xiaochouyulalala/RFhands/assets/70216817/086fcb6c-48b0-431b-a24e-8a0024976bcb)
