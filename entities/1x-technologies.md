---
title: 1X Technologies
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, robotics, embodiment, world-model]
sources: [raw/articles/soul2humanoid-report-1x-technologies.md, raw/articles/soul2humanoid-latest-news.md]
confidence: high
---

# 1X Technologies

2014 年成立（原名 Halodi Robotics），总部位于挪威奥斯陆 + 美国加州。OpenAI 领投 A/B 轮，累计融资超 $2.5 亿。

## 核心定位

**唯一主打家用市场的人形机器人公司**，直接面向 C 端消费者，而非工业场景。

## 硬件：NEO

- 身高 167cm / 体重 30kg / 行走 1.4m/s / 奔跑 6.2m/s
- **肌腱驱动（Tendon-Driven）**：反向可驱动性 95%，噪音仅 22dB
- **软体设计**：3D 晶格聚合物结构，外衣可机洗
- **计算**：NVIDIA Jetson Thor，最高 2070 FP4 TFLOPS
- 双 8.85MP 90Hz 鱼眼立体相机

## AI 架构

- **Redwood VLA**：移动 + 操作联合控制，从失败中学习
- **1X World Model**：基于物理的视频生成模型，执行前"想象"结果
- **内置 LLM**：离线语言模型，实时预测用户意图
- **Expert Mode**：用户预约 1X Expert 远程遥控，边做边学

## 制造

- **NEO Factory**（Hayward, CA）：58K sqft，全垂直整合
- Revo2 电机、电池、肌腱、22-DoF 手全部自产
- 初始产能 10,000 台/年，2027 年底目标 100,000 台/年
- 预售 5 天售罄

## 关系

- OpenAI 深度绑定，LLM 能力独特
- 与 [[nvidia-isaac]] 合作使用 Isaac Sim / Omniverse
- 与 [[figure-ai]]、[[tesla-optimus]] 目标市场不同（家用 vs 商业/工厂）
