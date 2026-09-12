# 我在用的 Skill 集合

[English](README.md) | **简体中文**

这是我日常配合 AI 编程和科研助手使用的科研技能集合，覆盖文献检索、论文写作与审稿、科研绘图、统计分析、生物信息学、分子建模和实验室工作流。

仓库收录了我手动安装的 **170 个工作流技能和 1 个共享依赖包**，保留了本地调整和上游作者署名，不包含助手内置技能及应用捆绑的插件技能。

## 按任务找技能

**[完整技能目录（英文）](CATALOG.md)** 列出了每个技能的简介、适用场景和许可证声明。需要程序化读取时，可使用 [catalog.json](catalog.json)。

| 我想做什么 | 可以从这些技能开始 |
|---|---|
| 检索论文、核对参考文献 | `paper-lookup`、`nature-academic-search`、`citation-management`、`nature-ref-verifier` |
| 精读论文、梳理实验与结论的关系 | `nature-paper-card`、`nature-reader`、`literature-review` |
| 设计研究、计算样本量 | `experimental-design`、`statistical-power`、`hypothesis-generation` |
| 起草、润色论文或回复审稿意见 | `nature-writing`、`nature-polishing`、`scientific-writing`、`nature-response` |
| 投稿前模拟审稿、检查统计报告 | `nature-reviewer`、`peer-review`、`nature-statistics` |
| 制作科研配图、海报或论文汇报 PPT | `nature-figure`、`scientific-visualization`、`scientific-slides`、`nature-paper2ppt`、`latex-posters` |
| 分析数据、建立统计或机器学习模型 | `statistical-analysis`、`pymc`、`scikit-learn`、`pytorch-lightning`、`polars` |
| 分析测序和单细胞数据 | `bulk-rnaseq`、`scanpy`、`scvi-tools`、`pydeseq2`、`pathway-enrichment` |
| 进行分子建模和药物发现研究 | `rdkit`、`deepchem`、`diffdock`、`molecular-dynamics`、`pkpd-modeling` |
| 连接实验室平台、记录实验过程 | `benchling-integration`、`opentrons-integration`、`pylabrobot`、`nature-experiment-log` |
| 协调从研究到论文的完整项目 | `academic-research-suite` |

## 如何使用

1. 打开所需技能的 `skills/<目录名>/SKILL.md`，查看适用范围、依赖和参考资料。
2. 将对应技能目录复制到你的 AI 助手支持的技能位置，或者让助手直接读取该目录中的 `SKILL.md`。
3. 保留目录中的脚本、参考资料、模板和素材。使用 Nature 系列技能时，如果它引用了 `skills/nature-shared`，请一并复制这个共享依赖包；其他兄弟技能依赖也按需保留。
4. 提供实际研究材料，并说明要完成的任务。例如：

```text
使用 nature-paper-card 分析这篇论文，梳理每项实验支持了哪些结论。
使用 nature-writing，根据这些图和测量结果起草 Results 部分。
使用 statistical-power，估算这项组间比较研究所需的样本量。
使用 scanpy 分析这份单细胞数据，并解释质控筛选的依据。
```

部分技能名称与目录名不同：例如 `researchwrite` 位于 `skills/nature-proposal-writer`。`nature-shared` 是供其他技能调用的依赖包，不是独立工作流。

仓库首页提供英文和简体中文版本，完整目录目前为英文。各技能内部保留原有的英文或中文指令，便于继续使用既有工作流和示例。

## 仓库内容

```text
skills/              科研技能目录及可复用资源
README.md            英文首页
README.zh-CN.md       中文首页
CATALOG.md           完整技能索引与适用场景（英文）
catalog.json         可供程序读取的索引
LICENSE.md           各组件许可证说明与上游来源
licenses/            保留的上游许可证文本
MODIFICATIONS.json   本地调整与发布前清理记录
EXCLUDED.md          未随仓库发布的技能及文件说明
```

这是我使用的技能集合快照，并不代表所有 API、软件包和助手集成都已安装或持续经过测试。部分在线工具需要单独的账号、API 密钥、数据访问权限或计算预算。仓库不包含凭据和私人研究输入。

## 来源与许可证

集合中的许多技能来自 [K-Dense 的 Scientific Agent Skills](https://github.com/K-Dense-AI/scientific-agent-skills)、[Nature Skills](https://github.com/Yuan1z0825/nature-skills) 和 [Academic Research Skills](https://github.com/Imbad0202/academic-research-skills)。本仓库整理这些材料并保留本地调整，不将上游技能声明为本人原创。

**不同组件适用的许可证可能不同。** 使用或再分发前，请查看 [LICENSE.md](LICENSE.md) 和对应技能自己的许可证说明。存在再分发限制或许可尚未明确的项目列在 [EXCLUDED.md](EXCLUDED.md) 中，没有使用统一许可证将它们重新发布。
