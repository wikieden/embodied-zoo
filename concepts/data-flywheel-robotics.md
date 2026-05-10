---
title: Data Flywheel in Robotics
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [training, robotics, self-supervised, multi-task]
sources: [raw/articles/soul2humanoid-report-figure-ai.md, raw/articles/soul2humanoid-report-tesla-optimus.md, raw/articles/soul2humanoid-report-physical-intelligence.md]
confidence: high
---

# Data Flywheel in Robotics

机器人部署 → 数据采集 → 模型训练 → 模型部署 → 更好的机器人行为 → 更多部署的闭环。

## 各公司飞轮模式

| 公司 | 飞轮模式 | 数据来源 | 强度 |
|------|----------|----------|------|
| **Tesla** | 车队级 | 数百万辆车 + 数千机器人 + YouTube 视频 | 极强 |
| **Figure AI** | BotQ 自主生成 | 仿真+真实混合 + 人类视频 | 强 |
| **Physical Intelligence** | π* 在线 RL | Open X-Embodiment + 自主 episode | 强 |
| **NVIDIA** | 平台级 | 生态反馈 + 合成数据 | 强 |
| **Boston Dynamics** | Fleet 共享 | Spot 2000+ 部署数据 | 中 |
| **1X** | 专家遥操作 | 真实家庭 + Expert 遥控 | 早期 |
| **Agility** | 监控为主 | 仓库部署数据 | 弱 |

## 最独特的数据策略

1. **Tesla FSD 迁移**：数百万辆车的驾驶数据直接用于机器人，任何竞争对手无法复制
2. **PI 跨本体数据**：用其他机器人的数据训练自己的策略，实现"数据杠杆"
3. **1X Expert Mode**：专家远程遥控解决家庭场景数据稀缺问题

## 合成数据的角色

- [[tesla-optimus]] "Digital Dreams"：Sora-like 视频生成 10,000+ 变体
- [[nvidia-isaac]] Omniverse Replicator：程序化生成无限标注数据
- [[physical-intelligence]] 世界模型：在仿真中试错再迁移到真实世界

## 关系

- 与 [[sim-to-real]] 紧密相关：数据飞轮的最终目标是缩小仿真-真实差距
- 与 [[vla-vision-language-action]] 相互依存：VLA 需要大规模数据，飞轮产生数据
