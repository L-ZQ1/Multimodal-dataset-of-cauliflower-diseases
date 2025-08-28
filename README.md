#Multimodal-dataset-of-cauliflower-diseases

一个高质量、专注于花椰菜病害的深度图像（Depth Image）数据集，旨在推动农业病害识别、植物健康监测和精准农业等领域的研究与应用。
📖 数据集简介
本数据集通过深度传感器（如Intel RealSense、微软Kinect或类似设备）采集，包含了健康与患病花椰菜在不同生长阶段、不同环境条件下的深度图像。深度图像提供了丰富的三维空间信息和表面结构细节，能够有效增强传统RGB图像在病害识别中的表现，特别适用于早期病害检测、严重程度评估和自动诊断系统的开发。


📊 数据详情

•​数据总量: 8,500 张深度图像
•​训练集: 6,000 张图像 (images/train/)
•​验证集: 1,500 张图像 (images/val/)
•​测试集: 1,000 张图像 (images/test/)
•​标注格式:
•​PASCAL VOC: 每张图像对应一个 .xml文件，包含边界框和病害类别信息
•​COCO: 统一的 annotations.json文件（可选格式）

•​病害类别:
•healthy_cauliflower- 健康花椰菜
•black_rot- 黑腐病
•downy_mildew- 霜霉病
•alternaria_leaf_spot- 黑斑病
•bacterial_soft_rot- 细菌性软腐病


🛠️ 下载与使用
1. 直接下载
您可以直接克隆或下载整个GitHub仓库。
bashbash复制git clone https://github.com/your-username/Deep-Image-Dataset.git
cd Deep-Image-Dataset



# 创建数据加载器
dataset = CauliflowerDiseaseDataset('images/train', 'annotations/train')
dataloader = DataLoader(dataset, batch_size=16, shuffle=True)


📝 标注信息
标注文件包含以下信息：

•​图像信息: 文件名、尺寸、采集日期
•​病害标注: 病害区域边界框坐标、病害类别、严重程度等级（可选）
•​环境信息: 光照条件、采集角度（可选）

🙏 引用
如果您在研究或项目中使用了本数据集，请通过以下方式引用：
bibtexbibtex复制@misc{DeepImageDatasetCauliflowerDisease,
  author = {您的姓名},
  title = {Deep Image Dataset: Cauliflower Disease Depth Imagery},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/your-username/Deep-Image-Dataset}}
}


📜 许可证
本项目采用 MIT License
        
      开源许可证。这意味着您可以自由地使用、修改和分发代码和数据集，但请附上原始许可证声明。
🤝 贡献
我们欢迎任何形式的贡献！

•报告错误或提出建议
•提交修复或改进的 Pull Request
•扩展数据集（请先开Issue讨论）
•添加新的病害类别或数据

💬 联系方式
如有任何问题，请通过以下方式联系：

•在 GitHub 仓库中 提交 Issue
•发送邮件至: 1484757741@qq.com
