---
title: Figure AI
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, model, robotics, embodiment]
sources: [raw/articles/soul2humanoid-report-figure-ai.md, raw/articles/soul2humanoid-latest-news.md]
confidence: high
---

# Figure AI

[官网](https://www.figure.ai) · [X/Twitter](https://x.com/Figure_robot)

估值 $390 亿的通用人形机器人公司，Helix VLA + BotQ 制造。

## 核心产品

- **Figure 03**：为量产、家庭、AI 设计的 173cm / 61kg 人形机器人，5h 续航
- **Helix VLA**：端到端视觉-语言-动作模型
  - Helix V1（2025.02）：上半身通才，35-DoF，200Hz
  - Helix 02（2026.01）：全身 loco-manipulation，三层时序架构
- **BotQ**：专用制造工厂，首代年产 12,000 台，四年目标 100,000 台

## Helix 三层架构

| 系统 | 频率 | 功能 |
|------|------|------|
| System 2 | 7 Hz | 语义/慢速推理："做什么" |
| System 1 | 200 Hz | 运动/中速控制："怎么做" |
| System 0 | 1 kHz | 执行/实时平衡："稳不稳" |

## 关键人物

- **Brett Adcock**：创始人（Archer / Vettery 连续创业者）

## 数据策略

1. 遥操作数据（500h）→ 2. 人体运动数据（1000h+）→ 3. 互联网规模人类视频（Project Go-Big，Brookfield 住宅环境）

## 关系

- 与 [[nvidia-isaac]] 合作使用 Isaac Sim 训练
- Helix 架构受 [[google-deepmind]] RT 系列启发
- 与 [[physical-intelligence]]、[[tesla-optimus]] 构成端到端 VLA 三强

> 来源：soul2humanoid-report-figure-ai.md, soul2humanoid-latest-news.md
