# Wiki Log

> 按时间顺序记录所有 wiki 操作。仅追加，不修改。
> 格式: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> 当本文件超过 500 条记录时，轮换: 重命名为 log-YYYY.md，重新开始。

## [2026-05-11] create | Wiki 初始化
- Domain: AI/具身大脑模型研究
- 结构已创建: SCHEMA.md, index.md, log.md
- 目录: raw/{articles,papers,transcripts,assets}, entities, concepts, comparisons, queries, _meta

## [2026-05-11] ingest | Soul2Humanoid 批量资料 ingest
- 来源: Soul2Humanoid GitHub 项目 raw/articles/ 下的 22 个文件
- 覆盖: 11 家具身智能公司报告 + 论文索引 + 横向对比 + 最新动态 + 资源
- 创建实体页面 (12):
  - entities/figure-ai.md
  - entities/physical-intelligence.md
  - entities/tesla-optimus.md
  - entities/boston-dynamics.md
  - entities/1x-technologies.md
  - entities/google-deepmind.md
  - entities/unitree.md
  - entities/nvidia-isaac.md
  - entities/apptronik.md
  - entities/agility-robotics.md
  - entities/enchanted-tools.md
  - entities/genesis-ai.md
- 创建概念页面 (10):
  - concepts/vla-vision-language-action.md
  - concepts/flow-matching.md
  - concepts/data-flywheel-robotics.md
  - concepts/sim-to-real.md
  - concepts/cross-embodiment.md
  - concepts/humanoid-robot.md
  - concepts/end-to-end-robotics.md
  - concepts/reinforcement-learning-robotics.md
  - concepts/imitation-learning-robotics.md
  - concepts/world-model-robotics.md
- 创建对比页面 (2):
  - comparisons/vla-architecture-comparison.md
  - comparisons/data-strategy-comparison.md
- 更新导航: index.md (24 页总数)

## [2026-05-11] ingest | GitHub 具身智能项目与研究方向全景 ingest
- 来源: `gh api` 搜索仿真器、VLA、Diffusion Policy、Sim2Real、开源硬件、人形运动等 10+ 类别
- 创建 raw 源: raw/articles/github-embodied-ai-projects-2026-05-11.md
- 创建概念页面 (1):
  - concepts/embodied-ai-research-landscape.md — 具身智能研究方向全景图（10个方向+开源项目+核心问题）
- 创建实体页面 (2):
  - entities/genesis-world.md
  - entities/lerobot.md
- 更新导航: index.md (27 页总数)
- 覆盖关键项目: Genesis, IsaacLab, LeRobot, Open X-Embodiment, SpatialVLA, Diffusion Policy, PACE, GMR 等

## [2026-05-11] ingest | 补充具身智能基准测试 (Benchmark)
- 来源: GitHub 搜索 embodied-benchmark, robot-benchmark, manipulation-benchmark, libero-benchmark
- 创建概念页面 (1):
  - concepts/embodied-benchmarks.md — 具身智能基准测试汇总：操作技能、长程任务、多智能体、跨本体等分类浏览
- 创建实体页面 (5):
  - entities/maniskill.md — SAPIEN GPU并行操作技能基准 (2860 ⭐)
  - entities/robosuite.md — Stanford 模块化操作仿真框架 (2405 ⭐)
  - entities/roboverse.md — 统一可扩展机器人学习平台 (1737 ⭐)
  - entities/metaworld.md — 多任务元强化学习基准 (1814 ⭐)
  - entities/robotwin.md — 双臂操作与数字孪生基准 (2299 ⭐)
- 更新概念页面 (1):
  - concepts/embodied-ai-research-landscape.md — 将基准测试单独列为第13个方向
- 更新导航: index.md (35 页总数)
- 关键项目覆盖: ManiSkill, robosuite, RoboTwin, MetaWorld, RoboVerse, LIBERO-plus, VMAS, PARTNR, VLA-Eval-Harness, LW-BenchHub, SoftGym, FluidLab, CausalWorld, GarmentLab, bigym, mshab, cap-x, EvoGym, InternManip

## [2026-05-11] update | 基准概念页面补充 GitHub 链接 + index 结构重构
- 为 4 个核心概念页面批量添加项目链接:
  - concepts/embodied-ai-research-landscape.md: +83 链接
  - concepts/embodied-benchmarks.md: +44 链接
  - concepts/long-horizon-reasoning.md: +16 链接
  - concepts/embodied-brain.md: +6 链接
  - 共计 +149 个 GitHub 链接
- index.md 重构:
  - Entities 分为 Companies (商业公司) 和 Open-Source Projects (开源项目与平台) 两个子分类
  - 新增 Research Directions (研究方向) 部分，列出 13 个方向并链接到对应概念页面
- 更新导航: index.md (35 页总数)