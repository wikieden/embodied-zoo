---
title: Boston Dynamics
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, robotics, locomotion, mpc, lab]
sources: [raw/articles/soul2humanoid-report-boston-dynamics.md, raw/articles/soul2humanoid-latest-news.md]
confidence: high
---

# Boston Dynamics

1992 年由 Marc Raibert 从 MIT Leg Laboratory 创立，足式机器人动态控制领域的全球领导者。2021 年被 Hyundai 以约 $11 亿收购。

## 产品矩阵

| 产品 | 形态 | 场景 | 部署规模 |
|------|------|------|----------|
| Spot | 四足 | 工业巡检 | 2,000+ |
| Stretch | 轮式+臂 | 仓储搬运 | 试点 |
| Atlas | 双足人形 | 制造/零件排序 | ~4 台/月（2026） |
| Orbit | 软件 | Fleet 管理 | — |

## Atlas 技术规格（产品版）

- 身高 1.9m / 体重 90kg / 56 DoF
- 关节**连续旋转**（无机械限位），超越人类运动范围
- 防护等级 IP67，工作温度 -20°C ~ 40°C
- 负载 50kg（瞬时）/ 30kg（持续），续航 4h

## AI 架构：分层混合

| 层级 | 方法 | 能力 |
|------|------|------|
| 底层平衡 | MPC + RL | 实时稳定、防滑、动态响应 |
| 中层运动规划 | 优化 + 学习 | 全身协调、避障、自碰撞避免 |
| 高层感知决策 | 视觉基础模型 + VLA | 语义理解、任务推理 |
| 操纵执行 | Diffusion Transformer（4.5亿参数） | 端到端灵巧操作、语言条件化 |

## 关键合作

- **TRI**（Toyota Research Institute）：联合发表论文，Atlas 使用单一 Diffusion Transformer 完成复杂长程操作
- **Google DeepMind**：Atlas AI 行为系统可能集成 Gemini Robotics

## 2026 危机

- CEO Robert Playter 退休、CTO Aaron Saunders 加入 DeepMind、VP Scott Kuindersma 离职
- Hyundai 要求年产 30,000 台，当前仅 ~4 台/月
- 研究→商业转型阵痛

## 关系

- 与 [[agility-robotics]] 同为**分层混合派**代表
- 与 [[google-deepmind]] 合作探索 VLA 集成
