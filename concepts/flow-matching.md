---
title: Flow Matching
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [model, architecture, robotics]
sources: [raw/articles/soul2humanoid-report-physical-intelligence.md, raw/articles/soul2humanoid-report-boston-dynamics.md]
confidence: high
---

# Flow Matching

一种连续时间生成模型，用于生成平滑、高频的连续动作轨迹。

## 核心特点

- 相比自回归或离散动作预测，能生成**更平滑、更高频**的连续动作
- 支持 **50Hz** 控制频率
- 适合机器人运动的连续性本质

## 应用例子

- [[physical-intelligence]] **π0**：3B VLM 骨干 + Flow Matching 动作专家
- [[boston-dynamics]] Atlas：Diffusion Transformer 使用 Flow Matching Loss，30Hz 控制频率

## 与 Diffusion 的关系

Flow Matching 是 Diffusion 模型的一种变体/简化，通过学习概率流的向量场（vector field）来生成数据。

## 关系

- 是 [[vla-vision-language-action]] 模型中动作生成的关键技术
- 与 [[reinforcement-learning-robotics]] 形成补充：RL 探索策略，Flow Matching 生成平滑轨迹
