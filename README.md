# Deep Image Dataset: Bell Pepper Depth Imagery

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)

一个高质量、专注于甜椒（Bell Pepper）的深度图像（Depth Image）数据集，旨在推动农业视觉、机器人采摘和3D形态分析等领域的研究。

## 📖 数据集简介

本数据集通过深度传感器（如Intel RealSense、微软Kinect或类似设备）采集，包含了在不同光照条件、不同成熟阶段和不同角度下拍摄的甜椒深度图像。深度图像提供了丰富的三维空间信息，是RGB图像之外的宝贵补充，非常适合用于实现精准的目标检测、实例分割、姿态估计和机器人抓取。

## 🗂️ 数据集结构

## 📊 数据详情

- **数据总量**: {例如: 5,000} 张深度图像
- **训练集**: {例如: 4,000} 张图像 (`images/train/`)
- **验证集**: {例如: 1,000} 张图像 (`images/val/`)
- **标注格式**:
  - **PASCAL VOC**: 每张图像对应一个 `.xml` 文件，包含边界框 (Bounding Box) 信息。
  - **COCO**: 一个统一的 `instances_train.json` 文件，包含所有目标检测信息。
- **类别**:
  本数据集目前仅包含一个类别：
  - `bell_pepper` (甜椒)

## 🛠️ 下载与使用

### 1. 直接下载
您可以直接克隆或下载整个GitHub仓库。
### 2. 在Python中加载 

## 📝 标注信息

标注文件包含以下信息：
- **文件名**: 对应的深度图像文件名。
- **图像尺寸**: 深度图像的宽度、高度和通道数（通常为1）。
- **物体信息**: 每个甜椒实例的边界框坐标 (`xmin, ymin, xmax, ymax`) 和类别标签。




## 🙏 引用

如果您在研究或项目中使用了本数据集，请通过以下方式引用：

## 📜 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。这意味着您可以自由地使用、修改和分发代码和数据集，但请附上原始许可证声明。

## 🤝 贡献

我们欢迎任何形式的贡献！
- 报告错误或提出建议
- 提交修复或改进的 Pull Request
- 扩展数据集（请先开Issue讨论）

## 💬 联系方式

如有任何问题，请通过以下方式联系：
- 在 GitHub 仓库中 [提交 Issue](https://github.com/{您的用户名}/Deep-Image-Dataset/issues)。
- 发送邮件至: {1484757741@qq.com}

---
**Happy Coding and Research!** 🚀
