---
title: Tesla Optimus
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, model, robotics, embodiment, end-to-end]
sources: [raw/articles/soul2humanoid-report-tesla-optimus.md]
confidence: high
---

# Tesla Optimus

Tesla 人形机器人项目，核心赌注是将 **FSD（全自动驾驶）端到端神经网络直接移植到人形机器人**。

## 核心架构

- **单一端到端神经网络**：拒绝 HTN、行为树、状态机，梯度从控制直接流向感知
- **FSD 技术迁移**：8 摄像头纯视觉、Occupancy Network、端到端路径规划、车队学习
- **Grok LLM**：xAI 的 Grok 3 提供自然语言理解和语音交互
- **VLA 统一网络**：视觉 + 语言 + 动作在一个网络中联合学习

## 数据来源（三级学习）

| 阶段 | 方法 | 数据来源 | 规模 |
|------|------|----------|------|
| Stage 1 | 遥操作 | 动作捕捉 + VR 头显 | 极低 |
| Stage 2 | 第一人称视频 | 内置 5 摄像头 POV | 中等 |
| Stage 3 | 互联网视频 | YouTube 等第三方视频 | 理论上无限 |

## 合成数据：Digital Dreams

生成式视频 AI（Sora-like）从单次真实演示生成 10,000+ 变体，解决模仿学习的数据瓶颈。

## 记忆机制

- **空间记忆**：环境建图与导航
- **车队集体记忆**：Cortex 超算（67,000+ H100）聚合全球机器人数据，OTA 推送
- **生成式世界记忆**：Neural World Simulator 可"想象"未来状态

## 当前能力边界

- ✅ 已解决：单步任务、低耦合任务、工厂重复性工作
- 🔄 演示级：扔垃圾、桌面清理、零件识别
- ❌ 未解决：完整备餐、杂乱房间找物品、洗碗机装载

## 关系

- 与 [[figure-ai]]、[[physical-intelligence]] 同为端到端派代表
- 数据飞轮规模全球第一（数百万辆车 + 数千机器人）
- 与 [[nvidia-isaac]] 在仿真领域有竞争/互补关系
