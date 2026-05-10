# Wiki Index

> 内容目录。每个 wiki 页面按类型列出，附带一行摘要。
> 查询时请先阅读本文件。
> Last updated: 2026-05-11 | Total pages: 39

## Entities
<!-- 按类型分类，内部按字母排列 -->

### Companies (商业公司)

- [[1x-technologies]] — OpenAI 投资的家用人形机器人公司，核心产品 NEO，肌腱驱动+世界模型
- [[agility-robotics]] — 物流仓储专用人形机器人 Digit，分层控制 LIPM+ZMP+MPC
- [[apptronik]] — 通用人形机器人平台 Apollo，硬件+合作 AI（Google Gemini）
- [[boston-dynamics]] — 1992 年创立的足式机器人领导者，Atlas/Spot/Stretch 产品线，分层混合架构
- [[enchanted-tools]] — 法国服务/社交场景机器人公司，产品 Miroki，Pepper/Nao 原班人马
- [[figure-ai]] — 估值 $390 亿的通用人形机器人公司，Helix VLA + BotQ 制造
- [[genesis-ai]] — 信息稀缺的新兴公司，声称 GENE-26.5 达到 Human-Level
- [[google-deepmind]] — 具身智能领域基石技术赋能者，RT-2/ππ-X/Gemini Robotics
- [[nvidia-isaac]] — 具身智能基础设施"卖铲人"，Isaac Sim/Lab + Jetson + GR00T
- [[physical-intelligence]] — 通用机器人策略π⁰/π⁰.7，Flow Matching + 跨本体，开源
- [[tesla-optimus]] — Tesla 人形机器人，FSD 神经网络直接移植，数据飞轮规模全球第一
- [[unitree]] — 中国宇树科技，$13,500 的 G1 人形机器人，极致性价比

### Open-Source Projects (开源项目与平台)

- [[genesis-world]] — 生成式物理世界仿真器，支持差分运算与大规模并行 (28.7k ⭐)
- [[lerobot]] — HuggingFace 端到端机器人学习框架，数据+训练+部署工具链 (23.9k ⭐)
- [[maniskill]] — GPU并行操作技能基准，基于 SAPIEN (2860 ⭐)
- [[metaworld]] — 多任务元强化学习基准，50 个操作任务 (1814 ⭐)
- [[robosuite]] — Stanford 模块化操作仿真框架 (2405 ⭐)
- [[roboverse]] — 统一可扩展机器人学习平台 (1737 ⭐)
- [[robotwin]] — 双臂操作与数字孪生基准 (2299 ⭐)

## Concepts

- [[cross-embodiment]] — 同一策略适配多种机器人形态的能力，Open X-Embodiment 和 π⁰ 为代表
- [[data-flywheel-robotics]] — 机器人部署→数据采集→训练→再部署的闭环，各公司飞轮模式对比
- [[differentiable-robotics]] — 可微分机器人学与基础工具：让物理、几何、运动学都可微分
- [[embodied-ai-research-landscape]] — 具身智能研究方向全景图，涵盖13个可投入方向与开源项目地图
- [[embodied-benchmarks]] — 具身智能基准测试汇总：操作技能、长程任务、多智能体、跨本体等分类浏览
- [[embodied-brain]] — 具身大脑架构：统一记忆、推理、情感、自我意识，让机器人成为能理解上下文的智能体
- [[end-to-end-robotics]] — 单一神经网络替代分层感知-规划-控制，Tesla/Figure/PI 为代表
- [[flow-matching]] — 连续时间生成模型，用于生成平滑高频连续动作轨迹
- [[humanoid-robot]] — 人形机器人定义、主流产品对比、技术分派概览
- [[imitation-learning-robotics]] — 机器人模仿学习，从遥操作到 YouTube 视频的三级演进
- [[long-horizon-reasoning]] — 长程任务推理：多步骤、长时间跨度、因果依赖的复杂任务规划与技能链接
- [[open-hardware-robotics]] — 开源硬件与低成本平台：降低具身智能研究的硬件门槛
- [[physics-simulators]] — 物理仿真器与数字孪生：具身智能的"训练场"
- [[reinforcement-learning-robotics]] — 强化学习在机器人中的应用，Isaac Gym/Lab 和企业实践
- [[robotics-data-engines]] — 数据集与数据引擎：机器人学习的"石油"
- [[sim-to-real]] — 仿真到真实的策略迁移，域随机化、域适应、残差策略学习
- [[vla-vision-language-action]] — 视觉-语言-动作统一模型架构，RT-2 定义的基础范式
- [[world-model-robotics]] — 机器人内心的物理世界预测模型，1X 和 Tesla 为代表

## Research Directions (研究方向)

<!-- 按全景图的 13 个方向归纳，链接到对应的概念页面 -->

1. [[physics-simulators]] — 物理仿真器与数字孪生：具身智能的"训练场"，仿真器保真度决定策略上限
2. [[robotics-data-engines]] — 数据集与数据引擎：机器人学习的"石油"，高质量多样化数据是瓶颈
3. [[vla-vision-language-action]] — VLA 模型架构：将视觉+语言理解映射到动作的统一范式
4. [[world-model-robotics]] — 世界模型：让机器人"在脑子里想"，预测未来观察与奖励
5. [[flow-matching]] — 动作生成 (Diffusion / Flow Matching / Transformer)：平滑高频连续动作轨迹
6. [[sim-to-real]] — Sim2Real 迁移与域适应：仿真训练策略无缝迁移到真实硬件
7. [[humanoid-robot]] — 人形机器人运动与全身控制：移动+操作+平衡的联合优化
8. [[open-hardware-robotics]] — 开源硬件与低成本平台：降低具身智能研究的硬件门槛
9. [[differentiable-robotics]] — 可微分机器人学与基础工具：让物理、几何、运动学都可微分
10. [[embodied-brain]] — 具身大脑：统一记忆、推理、情感、自我意识的认知架构
11. [[long-horizon-reasoning]] — 长程任务推理：多子目标、长时间跨度、因果依赖的复杂任务
12. [[cross-embodiment]] — 跨本体学习与泛化：同一策略适配多种机器人形态
13. [[embodied-benchmarks]] — 基准测试与评估：领域的"度量衡"

> 全景细节见 [[embodied-ai-research-landscape]]

## Comparisons

- [[data-strategy-comparison]] — 11 家公司数据来源、规模、飞轮模式与合成数据策略对比
- [[vla-architecture-comparison]] — 11 家公司 VLA 架构、基础模型、动作生成、跨本体能力对比

## Queries
<!-- 尚无已归档的查询结果 -->
