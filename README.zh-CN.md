<div align="right">

[English](README.md) | **简体中文**

</div>

# Cognitive Skills

**一组用于从基本事实形成认识、在真实情境中检验判断、设计有利轨迹，并将结果转化为可执行人际协作的 Agent Skills。**

Cognitive Skills 区分事实结构、情境判断、战略轨迹和人际行动。它们彼此相关，但不是同一个问题；每个 Skill 保持明确职责，同时可以按需组合。

## Skills

| Skill | 职责 | 适用场景 |
| --- | --- | --- |
| [`first-principles-dialogue`](skills/first-principles-dialogue/SKILL.md) | 从材料中提取原子事实与关系，组合并检验复杂命题 | 需要从现象、材料或想法重建认识结构时。 |
| [`situational-analysis`](skills/situational-analysis/SKILL.md) | 以五层五维检查问题结构和判断的全面性 | 一个局部成立的理解可能遗漏证据、系统、人性、时间或博弈时。 |
| [`strategic-analysis`](skills/strategic-analysis/SKILL.md) | 分析系统变化、反馈、互动与适应，设计更有利的轨迹 | 需要改善位置、寻找杠杆、预判回应或形成可适应策略时。 |
| [`communication-advisor`](skills/communication-advisor/SKILL.md) | 理解有明确目的的沟通局面，设计时机、对象、表达、边界和回应 | 工作、商业、服务、谈判、公开表达或一般社会互动需要改变理解与行动时。 |

这四个 Skills 不是必须依次执行的流水线。可以单独使用，也可以在需要更深入判断时组合使用：

1. 从材料中提取原子事实与关系，并形成可检验的候选命题；
2. 用五层五维检查这个问题和判断是否足够全面；
3. 分析局势怎样变化，以及怎样进入更有利的轨迹；
4. 将结果转化为可以执行的人际协作。

## 安装

使用 Skills CLI：

```bash
npx skills add hunterhigh/cognitive-skills
```

手动安装时，将 [`skills/`](skills/) 下任意一个完整目录复制到个人或项目级 Skills 目录。

## 使用

```text
使用 $first-principles-dialogue，从这些材料中提取原子事实和关系，再组合并检验候选命题。
使用 $situational-analysis，用五层五维检查这个问题的结构、遗漏和关键判断。
使用 $strategic-analysis，分析系统反馈、相关主体和演化路径，找出能够持续改善位置的策略。
使用 $communication-advisor，判断这次沟通的对象、时机、目的、表达和回应方式。
```

## 设计原则

- **推理先于表达。** 在优化结论如何呈现前，先暴露它所依赖的假设和证据。
- **语境会改变有效性。** 决策需要放进实际运行环境中检验，而不只是作为抽象论证评价。
- **沟通行动是独立层次。** 沟通会改变理解、承诺与行动，不只是给既有结论换一种表达。
- **保留不确定性。** 明确未知项、可逆行动以及可能改变决定的新证据。
- **软件包相互独立。** 每个 Skill 都有自己的入口，可以单独安装。

## 研究资料

- [Skill 体系第一轮迭代方案](docs/skill-system-iteration-plan.zh-CN.md)：围绕第一性原理、情境分析、战略分析、沟通顾问、项目构思、系统架构、项目连续性和目标纪律，定义本体、改动、验证与跨仓库实施顺序。
- [现实原理学习包](docs/reality-principles-learning-pack.zh-CN.md)：以 Dan Koe 的“研究现实本身”清单为入口，梳理系统、反馈、互动、适应、哲学与象征传统，并说明它们与本仓库及 Project Craft Skills 的关系和证据边界。
- [六个现实透镜：工程学习笔记](docs/reality-engineering-notes/README.md)：六篇第一人称长笔记，分别研究系统、控制、博弈、进化、热力学与螺旋动力学，并从 Skill ontology、接口、评价和演化角度检验它们对 Cognitive Skills 与 Project Craft 的工程价值。
- [优势系统研究](docs/reality-engineering-notes/07-advantage-system.md)：从六种现实透镜继续推导一套不预设中央主控、能够持续帮助用户寻找整体更优状态的 Skill 体系，并给出评价方式与可执行实验。
- [优势系统研究·第二章](docs/reality-engineering-notes/08-optimizing-skill-system.md)：从“持续生成更优状态”的原则回看 Cognitive Skills 与 Project Craft 的全部八个 Skill，提出可验证的收缩、补充和重构方向。

## 仓库结构

```text
skills/
├── first-principles-dialogue/
├── situational-analysis/
├── strategic-analysis/
└── communication-advisor/
```

## 验证

使用官方 Skill 验证器检查单个 Skill：

```bash
python /path/to/skill-creator/scripts/quick_validate.py skills/<skill-name>
```
