SwlFT-YOLO: A Frequency-Aware Lightweight Detector for Real-Time Tea Anthracnose Inspection on UAV-based Edge Devices

📌 论文状态 / Paper Status: Under Review

📌 Introduction

Welcome to the official repository for SwlFT-YOLO. This project presents a novel edge-tailored object detector built upon an inverted "Pruning-then-Tuning" cascade architecture and the Spatial-wavelet learnable Fusion Tuner (SwlFT) attention mechanism. It is designed to achieve highly accurate, low-latency, and real-time detection of early-stage tea anthracnose on UAV-based edge devices (e.g., NVIDIA Jetson Nano).

🚀 Current Repository Status

At present, this repository contains the following preliminary resources:

Pre-trained Weights: The fully trained model weight files (.pt) for SwlFT-YOLO.

Training Logs & Curves: The training process visualizations, including loss convergence curves, PR curves, and validation metrics (mAP@50: 75.8%).

⏳ Future Updates (Coming Soon)

To comply with double-blind peer-review policies and journal publishing guidelines, the complete source code will be released immediately after the paper is officially accepted and published. The upcoming release will include:

The complete YOLOv8-based model definition code with our custom structural modifications.

The core source code for the SwlFT attention mechanism, DownWT (Haar wavelet downsampling), and C2f_ScConv modules.

Complete training, validation, and inference scripts.

Python scripts for TensorRT engine serialization and edge device deployment (achieving 32.5 FPS on Jetson Nano).

Thank you for your interest and patience! Please feel free to ⭐ Star this repository to stay updated.

<h2 id="中文版">中文版</h2>

📌 项目简介

欢迎来到 SwlFT-YOLO 的官方代码仓库。本项目提出了一种专为边缘计算定制的新型目标检测器，它基于逆向的“先剪枝后微调（Pruning-then-Tuning）”级联架构以及 SwlFT（空间-小波可学习融合调优器）频域注意力机制。该模型旨在无人机搭载的边缘设备（如 NVIDIA Jetson Nano）上，实现对早期茶炭疽病的高精度、低延迟实时检测。

🚀 仓库当前状态

目前，本代码库已初步开源以下资源：

模型权重文件：SwlFT-YOLO 训练完成的最佳权重文件（包含 .pt）。

训练过程图表：完整的训练过程可视化数据，包括损失函数收敛图、PR曲线以及验证集评估指标（最终 mAP@50 达到 75.8%）。

⏳ 后续更新计划 (敬请期待)

为了严格遵守学术期刊的双盲审稿原则及出版规定，我们将在论文正式录用并发表后，第一时间全面公开所有的模型细节与完整源代码。

即将开源的内容包括：

包含完整结构改进的 YOLO 算法核心代码。

自定义模块的独家实现：SwlFT 频域注意力机制、DownWT 无损小波下采样以及 C2f_ScConv 模块。

完整的模型训练、验证和推理脚本。

基于 TensorRT 的边缘端 C++/Python 部署优化代码（在 Jetson Nano 上实测帧率达 32.5 FPS）。

感谢您的关注与耐心等待！欢迎点击右上角的 ⭐ Star 收藏本仓库以获取最新发布动态。
