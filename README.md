# RFhands
Deep Learning-based Hand Gesture Recognition Using Wireless RF Signals

![demo](https://github.com/xiaochouyulalala/RFhands/assets/70216817/5b16442e-9568-4702-95fc-c67e69bcb101)

## Abstract
This study presents RFhands, a novel hand keypoint recognition method that combines wireless radio frequency (RF) signals with deep learning to deliver a privacy-friendly solution that does not rely on visual sensors. The method transmits and receives raw RF signals through an antenna array, applies deep learning to extract meaningful features, and reconstructs hand keypoint data from those features. Experimental results show that RFhands performs well across diverse environments and gestures, achieving high accuracy and robustness. The system demonstrates the potential of RF-based gesture recognition as a privacy-preserving alternative to camera-based approaches, and extends the applicability of wireless sensing technology to a broader range of scenarios. Future research directions include further improving model accuracy and real-time performance, exploring additional application scenarios, and advancing RF signal processing techniques.

## Background
Gesture interaction is increasingly important in modern human-computer interaction. However, current camera-based gesture recognition systems suffer from privacy risks and sensitivity to lighting and occlusion. RF signal-based detection offers a compelling alternative: it protects user privacy, provides wide sensing coverage, is robust to occlusion and lighting variation, consumes less power, and can serve as an alternative or complementary input modality in mixed-reality devices.

## Research Goal
The goal of this research is to combine wireless RF signals with deep learning to propose RFhands, a novel hand keypoint recognition method, and to validate it through comprehensive experiments.

## Method
RFhands transmits and receives raw RF signals through an antenna array, then applies preprocessing and deep learning model analysis to construct a 3D hand skeleton model. The overall system architecture is an encoder-decoder structure: an RF signal deep neural network serves as the encoder, and a multi-layer fully connected network serves as the hand keypoint regression decoder.

![image](https://github.com/xiaochouyulalala/RFhands/assets/70216817/2b106a01-d06b-4e46-a472-f29889b892be)

## Experiments
This study uses a pipeline approach to collect RF and visual data, forming two primary datasets: a VR dataset and a general dataset. The RFhands model is implemented in PyTorch and trained on a cloud server with an NVIDIA RTX 3060 GPU. Model evaluation uses the VR gesture dataset and the general gesture dataset, with Percentage of Correct Keypoints (PCK) and Mean Per Joint Position Error (MPJPE) as the primary metrics.

![image](https://github.com/xiaochouyulalala/RFhands/assets/70216817/086fcb6c-48b0-431b-a24e-8a0024976bcb)
