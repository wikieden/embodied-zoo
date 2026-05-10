---
title: 长程任务推理
created: 2026-05-11
updated: 2026-05-11
type: concept
tags: [planning, cognition, embodiment, robotics, benchmark, model]
sources: [raw/articles/github-embodied-ai-projects-2026-05-11.md]
confidence: high
---

# 长程任务推理 (Long-Horizon Task Reasoning)

> 机器人需要完成涉及多个子目标、长时间跨度、因果依赖和世界状态变化的复杂任务。与短视程反射式控制不同，长程推理需要在动作之前或之中进行意图识别、序列规划和错误恢复。

## 问题定义

**短视程 vs 长程:**
- 短视程: "抓起红色方块"— 单一动作，即时反射
- 长程: "做一顿正餐"— 需要切菜→炒菜→盛盘→清理，每步都依赖前一步的状态

**核心难点:**
1. 组合爆炸: 子任务的排列组合随长度指数增长
2. 中间状态不确定性: 动作失败后需要重新规划
3. 目标层次化: 高层意图 (煮饭) 如何分解为低层动作 (打开炉火)
4. 因果推理: "如果先切菜再洗菜，菜会不新鲜"

## 关键开源项目与基准

**基准:**
- **[CALVIN](https://github.com/mees/calvin)** (910 ⭐) — 长程机器人操作语言条件策略学习基准，强调多步操作与语言指令结合
- **[BEHAVIOR-1K](https://github.com/StanfordVL/BEHAVIOR-1K)** (1457 ⭐) — 1000 种室内日常活动，大多数需要多步骤
- **[myGym](https://github.com/incognite-lab/myGym)** (53 ⭐) — 无代码生成多步长程任务，自动将基本动作组合成复杂流程

**策略方法:**
- **[Reflect-VLM](https://github.com/yunhaif/reflect-vlm)** (174 ⭐) — 反思式规划: VLM 用于多阶段长程操作
- **[Plan-Seq-Learn](https://github.com/mihdalal/planseqlearn)** (127 ⭐, ICLR'24) — LLM 引导的强化学习解决长程任务
- **[Action-Sketcher](https://github.com/FlagOpen/Action-Sketcher)** (48 ⭐, CVPR'26) — 通过视觉草图从推理到动作
- **[BUDS](https://github.com/UT-Austin-RPL/BUDS)** (57 ⭐) — 从未分段示教中自底向上发现技能
- **[Skill-Chaining](https://github.com/clvrai/skill-chaining)** (36 ⭐, CoRL'21) — 对抗技能链接用于长程操作
- **[PRoC3S](https://github.com/Learning-and-Intelligent-Systems/proc3s)** (31 ⭐, CoRL'24) — LLM + 约束满足解决长程问题
- **[LLaMAR](https://github.com/nsidn98/LLaMAR)** (32 ⭐) — 多智能体长程规划器

## 技术路线

| 方法 | 代表 | 特点 |
|------|------|------|
| 层级规划 (Hierarchical Planning) | [Plan-Seq-Learn](https://github.com/mihdalal/planseqlearn), [PRoC3S](https://github.com/Learning-and-Intelligent-Systems/proc3s) | LLM/高层意图 → 中层子任务 → 低层动作 |
| 技能链接 (Skill Chaining) | [BUDS](https://github.com/UT-Austin-RPL/BUDS), [Skill-Chaining](https://github.com/clvrai/skill-chaining) | 将短技能组合成长序列 |
| 反思与重规划 | [Reflect-VLM](https://github.com/yunhaif/reflect-vlm) | 执行中监控、失败时重新规划 |
| 视觉草图 | [Action-Sketcher](https://github.com/FlagOpen/Action-Sketcher) | 用图像表示中间目标和计划 |

## 开放问题

- **评估难题**: 如何量化"长程"的推理质量？仅看最终成功率会忽略中间过程
- **中间目标表示**: 如何让机器人自主发现或表示合适的中间目标？
- **错误恢复**: 一步失败后，是回退还是绕过？如何判断？
- **人类参考**: 人类如何处理长程任务？工作记忆还是脑中模拟？

## 与其他概念的关系

- [[embodied-brain]] — 长程推理是具身大脑的核心能力
- [[world-model-robotics]] — 世界模型支持对未来状态的预测，是规划的基础
- [[reinforcement-learning-robotics]] — RL 用于学习长程任务策略
- [[imitation-learning-robotics]] — 从人类演示中学习长程行为
- [[planning]] — 经典 AI 规划理论
