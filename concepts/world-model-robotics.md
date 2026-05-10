---
title: World Model for Robotics
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [world-model, model, robotics, planning]
sources: [raw/articles/soul2humanoid-report-1x-technologies.md, raw/articles/soul2humanoid-report-tesla-optimus.md]
confidence: medium
---

# World Model for Robotics

机器人内心对物理世界的"心理模拟"能力，能够预测动作结果。

## 主要实现

### 1X World Model

[[1x-technologies]] 的核心创新：

- 基于物理的视频生成模型
- 在真实执行前"想象"或"幻觉"出 NEO 动作的结果
- 允许机器人在仿真中试错，然后迁移到真实世界
- 能够泛化到从未见过的任务

### Tesla Neural World Simulator

[[tesla-optimus]] 的核心验证工具：

- 基于数百万辆车的驾驶数据训练
- 学习合成新的、高保真度的视频
- 可以生成 10,000+ 变体进行对抗测试
- 被理解为"生成式世界记忆"

### Physical Intelligence 隐形使用

[[physical-intelligence]] 的 π0.7 通过**视觉子目标**（Visual Subgoal Images）提供精确的空间布局信息，本质是世界模型的一种形式。

## 神经科学类比

世界模型概念上类似神经科学中的"预测处理"（predictive processing）理论——大脑不是被动感知世界，而是主动预测世界状态。

## 挑战

- **物理准确性**：视频生成模型很难精确预测物理交互
- **时间次度**：预测越远的未来越不准确
- **计算成本**：生成高保真度视频需要大量算力

## 关系

- 与 [[sim-to-real]] 重叠：世界模型可以理解为一种内部仿真器
- 与 [[vla-vision-language-action]] 结合：世界模型为 VLA 提供规划能力
