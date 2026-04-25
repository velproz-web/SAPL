# SAPL: Scale-Aware Progressive Learning for XCA Stenosis Segmentation

<div align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge" alt="License">
</div>

## 📖 项目简介 (Introduction)
本项目为**“面向X射线冠脉造影狭窄分割的尺度感知渐进式学习方法 (SAPL)”**的官方代码库。

在冠状动脉疾病的术中治疗中，X射线冠脉造影（XCA）的精准分割至关重要。针对现有网络难以兼顾“多尺度狭窄”与“极小尺寸病灶”的痛点，本项目提出了一种全新的 **尺度感知渐进学习 (Scale-Aware Progressive Learning, SAPL)** 框架。

本框架的核心创新点包括：
* **SCA (Scale-Aware Convolutional Aggregation)**: 尺度感知卷积聚合模块，有效捕捉多尺度敏感特征并抑制复杂背景干扰。
* **PFP (Progressive Feature Preservation)**: 渐进特征保留模块，通过特征选择与位置分配，从根本上缓解极小尺寸（直径<2mm）狭窄病灶的信息丢失问题。
* **SAL (Scale-Aware Loss)**: 尺度感知损失函数，根据狭窄尺度自适应调整权重。

实验表明，本模型在包含1500张XCA图像的ARCADE公共数据集上，F1分数及IoU等核心指标均显著优于现有主流方法。

## 🚀 最新动态 (Updates)
- [x] **模型架构与实验设计已完成** - [x] **竞赛技术报告已定稿**
- [ ] **核心网络代码 (Network Code) 整理中，即将开源**
- [ ] **预训练权重 (Pre-trained Weights) 即将上传**
- [ ] **快速推理演示脚本 (Demo Script) 编写中**

> **🔔 特别说明 (Notice):**
> **完整的数据预处理脚本、训练代码 (Train) 以及推理测试代码 (Inference) 将在近期（比赛网评结束后）陆续上传至本仓库，敬请期待！(The full source code will be released soon.)**

## 📊 效果预览 (Preview)
*(注：后续将在此处更新模型在S/M/L不同尺度下的可视化分割对比图。)*

## 🛠️ 环境依赖 (Requirements)
* Python >= 3.8
* PyTorch >= 1.10.0
* torchvision
* opencv-python
* numpy

## 📧 联系方式 (Contact)
本项目团队致力于智慧医疗与医学影像辅助诊断研究。如有技术交流需求，欢迎在本项目中提交 Issue。
