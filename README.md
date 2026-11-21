# SwlFT-YOLO

Code and weights for the manuscript "A UAV-borne edge computing system for tea anthracnose detection based on a frequency-aware lightweight model" (under review).

## Overview

SwlFT-YOLO is a YOLOv8n-based detector for symptomatic tea leaves, built to run onboard a UAV pod on an NVIDIA Jetson Orin Nano (8 GB). Its main component, the Spatial-Wavelet Learnable Fusion Tuner (SwlFT), refines learnable wavelet subbands alongside a spatial branch. Under the Fuse-then-Attend (FtA) placement, SwlFT sits after C2f fusion at the four neck nodes, where feature maps are narrower. The network also uses Haar wavelet downsampling (DownWT), C2f_ScConv and a BiFPN neck.

## Contents

- `SWlFT-YOLO.yaml`: model configuration (Ultralytics 8.3.68)
- `module/`: DownWT, C2f_ScConv and BiFPN implementations
- `Module Example/weights/`: trained weights (`best.pt`, `last.pt`)
- `Module Example/`: training curves and validation previews; best validation mAP@50 = 0.758 

Note: `best.pt` was trained with a single class. Parameter and FLOP counts in the paper are reported with the default 80-class head, following the official Ultralytics model cards.
ps: 'best.pt' requires the SwlFT module, which will be released after acceptance.

## Coming after acceptance

- SwlFT module source code
- Training, evaluation and inference scripts
- TensorRT FP16 export and Jetson deployment scripts
