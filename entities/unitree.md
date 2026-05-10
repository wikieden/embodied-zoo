---
title: Unitree 宇树科技
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, robotics, locomotion, reinforcement-learning, open-source]
sources: [raw/articles/soul2humanoid-report-unitree.md, raw/articles/soul2humanoid-latest-news.md]
confidence: high
---

# Unitree 宇树科技

[宇树科技](https://github.com/unitreerobotics) 2016 年成立于杭州，创始人王兴兴（1990 年生，上海大学硕士）。从四足机器人（机器狗）起家，2023 年切入人形机器人。

## 硬件产品

- **H1**：全尺寸人形，47kg（极致轻量化），行走速度 3.3m/s（世界纪录），189 N.m/Kg 扭矩密度
- **H1-2**：70kg，27 DoF，峰值负载 21kg
- **G1**：小型人形，$13,500 定价（"价格屠夫"），132cm / 35kg，面向教育/研究
- **R1 双臂平台**：$4,290 起，固定底座/轮式底座，15-31 DoF

## AI/控制

- **强化学习（RL）**驱动运动控制：行走、跑步、舞蹈（春晚《秧BOT》）
- **模仿学习**：动作捕捉 + 遥操作
- **UniFolm**：自研统一机器人大模型（跨四足+人形）
- 使用 [[nvidia-isaac]] Isaac Sim / Gym 训练

## 成本控制秘诀

1. 自研 M107 关节电机
2. 四足机器人量产经验摊薄研发成本
3. 中国制造供应链优势
4. 简化设计（G1 仅 5-DoF 手臂）

## 2026 动态

- 申请 $5.8 亿 IPO
- 年出货目标 20,000 台
- 王兴兴提出"80/80"目标：80% 任务 80% 成功率

## 关系

- 与 [[nvidia-isaac]] 深度合作（Jetson Orin、Isaac Sim）
- 价格定位与 [[figure-ai]]、[[boston-dynamics]] 形成鲜明对比
