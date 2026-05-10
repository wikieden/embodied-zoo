---
title: Physical Intelligence (π)
created: 2026-05-11
updated: 2026-05-11
type: entity
tags: [company, model, architecture, robotics, open-source]
sources: [raw/articles/soul2humanoid-report-physical-intelligence.md]
confidence: high
---

# Physical Intelligence (π)

致力于构建控制**任意机器人**完成**任意任务**的通用机器人基础模型。由学术明星团队创立，18 个月内完成 7 次重大迭代。

## 核心模型演进

| 时间 | 版本 | 突破 |
|------|------|------|
| 2024.10 | π0 | 首个通用跨本体策略，VLM + Flow Matching，8 种机器人 |
| 2025.01 | FAST | DCT + BPE 动作 tokenization，10x 压缩，5x 加速 |
| 2025.02 | 开源 | π0 + FAST 权重与代码开源 |
| 2025.11 | π*0.6 / Recap | 首个在线 RL 训练的通用策略 |
| 2026.03 | MEM + RLT | 多尺度具身记忆（15min 长程）+ 高效 RL Token |
| 2026.04 | π0.7 | 可组合泛化，涌现技能重组能力 |

## 六大研究方向

1. **通用 VLA 基础模型**：3B VLM + Flow Matching 动作专家，50Hz 连续控制
2. **FAST 动作表示**：DCT 频域压缩 + BPE 子词编码，使自回归 VLA 成为可能
3. **跨本体迁移**：同一策略控制单臂/双臂/移动底盘，零样本迁移到新机器人
4. **RL 自提升闭环**：通用策略 → 在线 RL 优化 → 蒸馏回通用策略
5. **MEM 多尺度记忆**：短期视觉记忆 + 长期语言记忆，支持 15 分钟长程任务
6. **实时性优化**：Real-Time Chunking、Knowledge Insulation、RLT

## 关键优势

- **开源生态**：[π0](https://github.com/Physical-Intelligence/openpi) 和 [FAST](https://github.com/Physical-Intelligence/fast) 开源，成为学术界基准
- **跨本体泛化**：在 UR5e 双臂上零样本完成折叠衣物（从未在该机器人上训练）
- **数据杠杆**：直接基于 [[google-deepmind]] 的 Open X-Embodiment 数据集训练

## 关系

- 与 [[google-deepmind]] 间接依赖（数据集）
- 与 [[figure-ai]]、[[tesla-optimus]] 构成端到端 VLA 三强，但 PI 专注通用策略而非自有硬件
