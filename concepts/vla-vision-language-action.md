---
title: VLA (Vision-Language-Action)
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [model, architecture, multimodal, robotics]
sources: [raw/articles/soul2humanoid-papers.md, raw/articles/soul2humanoid-report-figure-ai.md, raw/articles/soul2humanoid-report-physical-intelligence.md]
confidence: high
---

# VLA (Vision-Language-Action)

将视觉感知、语言理解和动作生成统一在单一模型中的架构范式。

## 历史

[[google-deepmind]] 的 **RT-2**（2023.07）首次将大规模视觉-语言模型（PaLI-X/PaLM-E）直接输出机器人动作 token，被引用 2000+ 次，成为具身智能基石论文。

## 架构组成

| 组件 | 功能 | 代表技术 |
|------|------|----------|
| 多模态输入 | 感知环境 + 任务指令 | 相机图像、自然语言、动作历史 |
| VLM 骨干 | 语义理解与知识迁移 | 3B 参数预训练视觉-语言模型 |
| 动作专家 | 生成高频连续动作 | Flow Matching / Diffusion / 自回归 |

## 动作表示方法

- **离散 token**：RT-2 将动作离散化为 256 个 token
- **Flow Matching**：生成平滑连续动作轨迹（[[physical-intelligence]] π0 采用）
- **FAST**：DCT + BPE 动作 tokenization，10x 压缩率

## 主流实现

| 公司 | 模型 | 动作生成 | 特点 |
|------|------|----------|------|
| Figure AI | Helix | 双系统（快/慢） | 全身 loco-manipulation |
| Physical Intelligence | π0 | Flow Matching 50Hz | 跨本体 8 种机器人 |
| Tesla | Optimus VLA | 端到端直接输出 | FSD 技术迁移 |
| Google DeepMind | Gemini Robotics | 动作 token | 双模型 VLA+ER |

## 挑战

- **实时性**：大模型推理延迟 vs 机器人 50-200Hz 控制需求
- **数据瓶颈**：机器人数据集远小于视觉-语言数据
- **安全验证**：端到端黑箱难以形式化验证

## 关系

- 定义者：[[google-deepmind]] RT-2
- 开源基准：[[physical-intelligence]] π0
- 行业数据基础：[[google-deepmind]] Open X-Embodiment
