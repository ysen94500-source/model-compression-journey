# Model Compression Journey

> 模型压缩与边缘 AI 部署学习记录 — 从理论到瑞芯微 RK3588 NPU 实战

## About

本仓库记录我在模型压缩与边缘部署方向的系统性学习过程，涵盖量化、剪枝、知识蒸馏、稀疏化等核心技术，以及 ONNX / RKNN / TensorRT 工具链的实战经验。

**背景：** 南京师范大学 AI 学院硕士，研究方向为基于黎曼几何的 EEG 癫痫检测与边缘部署。在研究中实现了 700× 计算量压缩（45M → 65k MACs）且精度不降反升，由此对模型压缩产生了深入的兴趣和实践动力。

## Repository Structure

```
├── notes/                    # 学习笔记
│   ├── 01_quantization_basics.md
│   ├── 02_ptq_vs_qat.md
│   └── ...
├── experiments/              # 实验代码与结果
│   ├── mnist_ptq/            # MNIST 训练后量化实验
│   ├── resnet_qat/           # ResNet QAT 实验
│   └── ...
├── projects/                 # 完整项目（独立仓库的索引）
└── benchmarks/               # 性能基准测试数据
```

## Learning Roadmap

| Phase | Period | Focus | Status |
|-------|--------|-------|--------|
| 0 | 2026.06 | 量化理论 + 环境搭建 + 首个量化实验 | 🔄 In Progress |
| 1 | 2026.07-08 | PTQ/QAT 进阶 + RKNN 实战 + C++ 入门 | ⬜ Planned |
| 2 | 2026.09-12 | EEG 模型压缩部署到 RK3588 NPU | ⬜ Planned |
| 3 | 2027.01-03 | 知识蒸馏 + LLM 量化 + 工具链对比 | ⬜ Planned |

## Tech Stack

- **Frameworks:** PyTorch, ONNX
- **Compression:** Quantization (PTQ/QAT), Pruning, Knowledge Distillation
- **Deployment:** RKNN-Toolkit2, TensorRT, ONNX Runtime
- **Hardware:** Rockchip RK3588 (Orange Pi 5), STM32 MCU
- **Languages:** Python, C++

## Related Projects

- 🔬 **EEG-Seizure-Detection-RK3588** — 基于黎曼几何的癫痫检测模型在 RK3588 NPU 上的完整压缩部署 (coming soon)
- 🚀 **YOLOv8-RK3588-Deploy** — YOLOv8 目标检测模型的 RKNN 部署实战 (coming soon)

## Notes Index

> 持续更新中，每周至少一篇。

| # | Title | Date | Tags |
|---|-------|------|------|
| 01 | 量化从零理解：从浮点到定点 | - | `quantization` `basics` |

---

*This repository is part of my journey toward becoming a model compression engineer, bridging the gap between academic research and industrial edge AI deployment.*
