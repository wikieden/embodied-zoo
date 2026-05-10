---
title: NVIDIA Isaac
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, robotics, sim-to-real, training, inference]
sources: [raw/articles/soul2humanoid-report-nvidia-isaac.md]
confidence: high
---

# NVIDIA Isaac

NVIDIA 的具身智能基础设施平台，**"卖铲人"定位**——不造机器人本体，提供芯片+仿真+训练+部署全栈工具。

## 平台架构

| 层级 | 产品 | 功能 |
|------|------|------|
| 应用层 | GR00T | 人形机器人基础模型参考设计 |
| 训练层 | Isaac Lab | RL + 模仿学习 + Sim2Real |
| 仿真层 | Isaac Sim / Omniverse | 物理仿真 + 传感器模拟 |
| 计算层 | Jetson / DGX / H100 | 边缘推理 + 云端训练 |
| 本体层 | 参考设计 + 合作伙伴 | Figure、1X、Agility、BD 等 |

## 核心组件

- **Isaac Sim**：基于 Omniverse/USD，GPU 加速，支持数千环境并行
- **Isaac Lab**：统一 RL/IL 训练框架，兼容 PyTorch / Hugging Face LeRobot
- **Jetson Thor**：2024 年发布，专为机器人设计，集成 Transformer Engine
- **Omniverse Replicator**：程序化生成无限标注合成数据
- **Project GR00T**：Transformer VLA 参考模型

## 竞争优势

- **计算垄断**：GPU 是 AI 训练唯一选择，Jetson 是边缘 AI 首选
- **生态绑定**：几乎所有机器人公司都依赖 NVIDIA 硬件/软件
- **合成数据工厂**：解决机器人领域数据瓶颈

## 飞轮效应

越多公司用 Isaac → 越多真实数据反馈 → 仿真器越逼真 → 合成数据质量越高 → 模型越强 → 越多公司用 Isaac

## 关系

- 与 [[figure-ai]]、[[1x-technologies]]、[[unitree]]、[[boston-dynamics]]、[[apptronik]]、[[agility-robotics]] 均为合作伙伴
- 与开源仿真器（MuJoCo、Genesis）形成竞争
