# OPMMDoctor

**Multimodal Deep-Learning Model for Opportunistic Osteoporosis Screening Using Whole-Body Multi-Joint Radiographs and Clinical Indicators**

OPMMDoctor 是一套融合全身多关节 X 线影像与结构化临床指标的多模态深度学习框架，用于骨质疏松症机会性筛查。框架由四个核心模块组成：

- **图像特征提取分支**：Swin Transformer V2 提取多尺度骨骼特征；
- **临床特征编码分支**：对结构化临床指标进行正弦数值编码；
- **临床-视觉融合模块（CVFM）**：区域跨模态调制 + 可靠性感知门控，实现异构模态自适应融合；
- **专家引导有序损失模块（EGOLM）**：面向有序三分类的损失设计，降低跨级高风险误判。

## ⚠️ Code Availability / 代码开放说明

> **The full source code and trained weights will be publicly released here upon acceptance of the manuscript.**
>
> 完整源代码与训练权重将在论文**被接收后**在本仓库公开。当前仓库仅提供项目说明与目录结构占位。

## Repository Structure / 目录结构

```
OPMMDoctor/
├── README.md
├── requirements.txt        # 依赖列表（占位）
├── docs/                   # 文档：方法、架构、使用说明
│   ├── overview.md
│   └── architecture.md
├── src/                    # 源代码（接收后公开）
│   ├── README.md
│   └── models/
└── data/                   # 数据说明（不含受限的患者数据）
    └── README.md
```

## Citation / 引用

If you find this work useful, please cite the paper (details to be updated upon publication).

## Contact

Corresponding authors: see the manuscript.
