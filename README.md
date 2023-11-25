# SASAN: Spectrum-Axial Spatial Approach Networks for Medical Image Segmentation

### [Project page](https://github.com/IIPL-HangzhouDianziUniversity/SASAN-pytorch) | [Our laboratory home page](https://github.com/IIPL-HangzhouDianziUniversity) 

SASAN: Spectrum-Axial Spatial Approach Networks for Medical Image Segmentation

Xingru Huang, Jian Huang, Kai Zhao, Tianyun Zhang, Zhi Li, Changpeng Yue, Wenhao Chen, Ruihao Wang, Xuanbin Chen, Yaoqi Sun, Juzhen Wang, and Yihao Guo

Hangzhou Dianzi University

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/SASAN-pytorch/blob/main/figures/SASAN.png">
</div>
<p align=center>
  Figure 1: The network structure of SASAN.
</p>

We proposed SASAN, a novel 3D medical image segmentation network, and our approach achieved state-of-the-art performance compared to 13 previous segmentation methods.

We will first introduce our method and principles, then introduce the experimental environment and provide Github links to previous methods we have compared. Finally, we will present the experimental results and our pre-trained model.

## Methods
### FINE Module

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/SASAN-pytorch/blob/main/figures/FINE.png"width=80% height=80%>
</div>
<p align=center>
  Figure 2: The FINE Module.
</p>

FINE combines spatial and frequency domain information to add low-frequency details from the original image to the feature map. This preserves the main structural information and effectively reduces noise and other disturbances.

### ASEM Module

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/SASAN-pytorch/blob/main/figures/ASEM.png">
</div>
<p align=center>
  Figure 3: The ASEM Module.
</p>

ASEM comprehensively extracts spatial features and features along each axis of 3D OCT sequences, significantly enhancing the network's analytical capabilities.

## Installation
We run SASAN and previous methods on a system running Ubuntu 22.04, with Python 3.9, PyTorch 2.0.0, and CUDA 11.8. For a full list of software packages and version numbers, see the experimental environment file `environment.yml`. 

## Experiment
### Baselines

[3D U-Net](https://github.com/wolny/pytorch-3dunet); [RAUNet](https://github.com/nizhenliang/RAUNet); [UNETR](https://github.com/tamasino52/UNETR); [SwinUNETR](https://github.com/LeonidAlekseev/Swin-UNETR); [ResUNet](https://github.com/rishikksh20/ResUnet);
[MultiResUNet](https://github.com/nibtehaz/MultiResUNet); [V-Net](https://github.com/mattmacy/vnet.pytorch); [3D UX-Net](https://github.com/MASILab/3DUX-Net); [SegResNet](https://github.com/Project-MONAI/MONAI/blob/dev/monai/networks/nets/segresnet.py); [HighRes3DNet](https://github.com/fepegar/highresnet);
[TransBTS](https://github.com/Rubics-Xuan/TransBTS); [nnFormer](https://github.com/282857341/nnFormer); [SETR](https://github.com/fudan-zvg/SETR)

We have provided GitHub links pointing to the PyTorch implementation code for all networks compared in this experiment so you can easily reproduce all these projects.

### Training Results






