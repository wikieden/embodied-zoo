---
title: Imitation Learning in Robotics
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [imitation-learning, training, robotics]
sources: [raw/articles/soul2humanoid-report-tesla-optimus.md, raw/articles/soul2humanoid-report-figure-ai.md]
confidence: high
---

# Imitation Learning in Robotics

机器人通过模仿人类演示数据来学习任务。

## Tesla 的三级模仿学习

| 阶段 | 方法 | 规模 | 时间 |
|------|------|------|------|
| Stage 1 | 遥操作（动作捕捉 + VR） | 极低 | 2022-2024 |
| Stage 2 | 第一人称视频（内置 5 摄像头） | 中等 | 2025 中期 |
| Stage 3 | 互联网视频（YouTube 等） | 无限（理论） | 2025+ |

> "If Optimus can watch YouTube videos and learn to do that thing... you really have task extensibility that is dramatic."
> — Elon Musk

## 其他公司的模仿学习

- [[figure-ai]]：~500h 高质量遥操作数据，VLM 自动生成 hindsight 指令
- [[physical-intelligence]]：人类视频到机器人任务的迁移能力在规模上涌现
- [[boston-dynamics]]：人类遥操作（VR/平板）提供高质量种子数据
- [[1x-technologies]]：Expert Mode 专家遥控，边做边学

## 与 RL 的对比

| | 模仿学习 | 强化学习 |
|--|----------|----------|
| 数据来源 | 人类演示 | 自主试错 |
| 学习速度 | 快（直接学习有效行为） | 慢（需要大量探索） |
| 遭遇的场景 | 受限于演示覆盖范围 | 可以探索未知场景 |
| 安全性 | 高（不会尝试危险行为） | 低（需要安全约束） |
| 精度 | 受限于演示精度 | 可以超越人类演示 |

## 关系

- 常与 [[reinforcement-learning-robotics]] 组合：IL 初始化 + RL 微调
- Tesla 的合成数据"数字梦境"将 IL 与生成式 AI 结合
