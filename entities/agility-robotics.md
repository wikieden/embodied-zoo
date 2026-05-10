---
title: Agility Robotics
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, robotics, locomotion, manipulation]
sources: [raw/articles/soul2humanoid-report-agility-robotics.md]
confidence: high
---

# Agility Robotics

2015 年成立于俄勒冈州立大学 spin-off。核心产品 Digit，定位**物流/仓储场景专用人形机器人**。

## 设计哲学

- **场景优先**：完全围绕"搬运塑料 tote"优化，非通用设计
- **成本可控**：无五指灵巧手、无躯干自由度，硬件复杂度低
- **热插拔电池**：1-2 分钟更换，支持连续作业

## Digit 2.0 规格

- 身高 ~175cm / 体重 ~65kg / 16 DoF / 行走 1.5m/s
- 负载 ~16kg（单 tote）/ 续航 2-4h
- 头部 Intel RealSense 深度相机

## AI 架构：传统分层控制

| 层级 | 方法 | 功能 |
|------|------|------|
| 任务调度 | WMS 集成 | 接收搬运指令 |
| 高层规划 | 路径规划 | 避障、抓取策略 |
| 运动控制 | LIPM + ZMP + MPC | 双足动态行走 |
| 底层关节 | PD + 力矩前馈 | 关节控制 |

- 预定义步态库，非神经网络生成
- 视觉伺服定位 tote，力/位置混合控制夹爪

## 商业化

- 与 **Amazon** 仓库试点（2022-2023）
- 与 **GXO** 签订多年合作协议（2024）
- 2026 年 Peggy Johnson 新任 CEO，提出"Unconstrained Humanoids"愿景

## 关系

- 与 [[boston-dynamics]] 同为**分层混合派**代表
- 与 [[google-deepmind]] 合作（可信测试者，Digit 集成 Gemini）
