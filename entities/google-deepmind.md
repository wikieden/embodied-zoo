---
title: Google DeepMind
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [lab, model, architecture, open-source]
sources: [raw/articles/soul2humanoid-report-google-deepmind.md, raw/articles/soul2humanoid-papers.md]
confidence: high
---

# Google DeepMind

[官网](https://deepmind.google) · [X/Twitter](https://x.com/GoogleDeepMind) · [GitHub](https://github.com/google-deepmind)

具身智能领域最重要的**技术赋能者**，不造硬件，纯软件/模型。定义了 VLA 架构，构建了行业数据基础设施。

## 技术演进

| 时间 | 技术 | 贡献 |
|------|------|------|
| 2023.07 | RT-2 | 首个大规模 VLA，VLM 直接输出机器人动作 token |
| 2023.10 | RT-X / Open X-Embodiment | 全球最大跨机器人数据集，22 种形态、1600万+ 轨迹 |
| 2024.03 | RT-H | 语言描述中间步骤，提升长程任务成功率 |
| 2024.08 | Gemini Robotics | Gemini 多模态能力引入机器人控制 |
| 2026.04 | Gemini Robotics-ER 1.6 | 增强具身推理，支持复杂任务规划 + 工具使用 |

## 双模型架构

- **Gemini Robotics 1.5（VLA）**：看 + 理解 + 动，跨本体泛化
- **Gemini Robotics-ER 1.6（具身推理）**：物理世界推理、逻辑决策、任务规划

## 开源贡献

- **[Open X-Embodiment Dataset](https://github.com/google-deepmind/open_x_embodiment)**：全球 20+ 研究机构联合，被 [[physical-intelligence]] [π0](https://github.com/Physical-Intelligence/openpi)、[[figure-ai]] Helix 等直接使用
- [RT-2](https://github.com/google-deepmind/rt2) / RT-X 论文被引用数千次，具身智能基石文献

## 合作伙伴生态

| 公司 | 合作类型 |
|------|----------|
| Apptronik | 共建下一代人形机器人 |
| Boston Dynamics | Atlas 集成 Gemini |
| Agility Robotics | Digit 集成 Gemini |
| Figure AI | 间接（技术参考） |
| Physical Intelligence | 间接（数据集） |

## 关系

- 与 [[physical-intelligence]] 形成对比：平台赋能者 vs 垂直整合
- 几乎所有主流机器人公司都在使用或参考其技术
