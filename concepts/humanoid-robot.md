---
title: Humanoid Robot
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [robotics, embodiment, locomotion, manipulation]
sources: [raw/articles/soul2humanoid-index.md, raw/articles/soul2humanoid-comparisons.md]
confidence: high
---

# Humanoid Robot

拥有类人形态（双足、双臂、头部、躯干）的机器人，设计初衷是适配人类现有环境。

## 为什么是人形

- **环境通用性**：无需为每种任务改造环境，一个形态服务数百万种任务
- **视角相似性**：运动学和视角与人类相似，便于从人类视频迁移知识
- **社会接受度**：人类对类人形态有本能的亲和感

## 主流产品对比

| 公司 | 产品 | 身高 | 体重 | DoF | 价格/定位 | 市场 |
|------|------|-------|-------|-----|------------|------|
| Figure AI | Figure 03 | 173cm | 61kg | ~35+ | $400-600/月租赁 | 商业→家庭 |
| Boston Dynamics | Atlas | 190cm | 90kg | 56 | 未公开 | 工业 B2B |
| Tesla | Optimus | ~173cm | ~73kg | ~78 | 未公开 | 工厂→家庭 |
| 1X | NEO | 167cm | 30kg | ~30+ | 未公开 | 家庭 C 端 |
| Unitree | H1 | 180cm | 47kg | ~20 | 不是消费级 | 教育/研究 |
| Unitree | G1 | 132cm | 35kg | 23 | $13,500 | 教育/研究 |
| Agility | Digit | 175cm | 65kg | 16 | 未公开 | 仓储 B2B |
| Apptronik | Apollo | 173cm | 73kg | ~30+ | 未公开 | 工业 B2B |

## 技术分派

- **端到端派**：[[figure-ai]]、[[physical-intelligence]]、[[tesla-optimus]]
- **分层混合派**：[[boston-dynamics]]、[[agility-robotics]]
- **平台+合作 AI**：[[apptronik]]、[[enchanted-tools]]

## 关系

- AI 大脑：[[vla-vision-language-action]]
- 训练基础：[[sim-to-real]]
- 数据驱动：[[data-flywheel-robotics]]
