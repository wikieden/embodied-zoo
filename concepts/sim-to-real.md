---
title: Sim-to-Real Transfer
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [sim-to-real, training, robotics, reinforcement-learning]
sources: [raw/articles/soul2humanoid-report-nvidia-isaac.md, raw/articles/soul2humanoid-report-unitree.md, raw/articles/soul2humanoid-report-figure-ai.md]
confidence: high
---

# Sim-to-Real Transfer

将在仿真环境中训练的策略迁移到真实机器人上的技术。

## 核心方法

| 方法 | 原理 | 应用 |
|------|------|------|
| **Domain Randomization** | 仿真中随机化纹理、光照、摩擦、质量 | 提高策略对真实环境变化的鲁棒性 |
| **Domain Adaptation** | GAN/自适应网络缩小仿真-真实差距 | 修正仿真器偏差 |
| **System Identification** | 识别真实机器人动力学参数 | 使仿真更精确 |
| **Residual Policy Learning** | 仿真策略 + 真实世界微调 | 快速适应特定硬件 |

## 主流仿真器

| 平台 | 特点 | 用户 |
|------|------|------|
|| [[nvidia-isaac]] [Isaac Sim](https://github.com/NVIDIA-Omniverse/IsaacSim) | GPU 并行、Omniverse/USD 生态 | Figure、1X、Unitree |
|| [MuJoCo](https://github.com/google-deepmind/mujoco) | 开源、精确控制系统仿真 | 学术界、Boston Dynamics |
|| [Genesis](https://github.com/Genesis-Embodied-AI/Genesis) | 开源、极速仿真 | 学术界（与 Genesis AI 无关） |

## 企业实践

- [[unitree]]：春晚《秧BOT》高动态舞蹈由 RL 在 Isaac Sim 中训练，零样本迁移
- [[figure-ai]]：System 0 全身控制器在仿真中训练，零样本楼梯/不平地面行走
- [[tesla-optimus]]：Neural World Simulator 生成数千个变体进行 RL 训练

## 挑战

- 物理差异：仿真器难以完美复刻真实世界的接触力学
- 视觉差异：仿真相机 vs 真实相机的光照、噪声、镜头失真
- 接触动力学：摩擦、弹性、可变形物体

## 关系

- 与 [[data-flywheel-robotics]] 互补：仿真数据是飞轮的重要组成部分
- 与 [[reinforcement-learning-robotics]] 紧密绑定：RL 主要在仿真中训练
