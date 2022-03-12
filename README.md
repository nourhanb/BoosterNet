# BoosterNet
This is the official implementation of CVPR2022 "**BoosterNet: Improving Domain Generalization of Deep Neural Nets using Culpability-Ranked Features**"

## Overview
BoosterNet is a lean add-on network that can be simply appended to any arbitrary core network to improve its generalization capability without requiring any changes in its architecture or training procedure. Using a novel measure of feature culpability, BoosterNet is trained on the most and least culpable data features extracted from critical units in the core network based on their contribution towards class-specific prediction errors. At inference time, corresponding test image features are extracted from the closest class-specific units, determined by smart gating via a Siamese network, and fed to BoosterNet for improved generalization. 

