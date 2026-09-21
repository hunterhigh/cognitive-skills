<div align="right">

[English](README.md) | **简体中文**

</div>

# Cognitive Skills

**一组用于回到基本事实、在真实情境中作出判断，并将判断转化为可执行人际协作的 Agent Skills。**

Cognitive Skills 建立在一个简单区分之上：可靠的前提、可靠的决定和可靠的工作行动彼此相关，但并不是同一个问题。本仓库让它们各自保持明确职责，同时可以按需组合。

## Skills

| Skill | 职责 | 适用场景 |
| --- | --- | --- |
| [`first-principles-dialogue`](skills/first-principles-dialogue/SKILL.md) | 将命题拆解为事实、假设、定义和推理关系 | 需要从第一性原理审视某个概念或复杂命题时。 |
| [`situated-decision`](skills/situated-decision/SKILL.md) | 用证据、语境、利益、不确定性和变化检验判断 | 一个局部成立的方案可能在更大的现实系统中失效时。 |
| [`work-alignment-advisor`](skills/work-alignment-advisor/SKILL.md) | 将判断转化为与他人的明确承诺、边界、沟通和下一步 | 问题涉及与领导、同事、客户或合作方对齐时。 |

这三个 Skills 不是必须依次执行的流水线。可以单独使用，也可以在需要更深入判断时组合使用：

1. 确认命题建立在什么事实和假设之上；
2. 检查这个判断放入真实情境后是否仍然成立；
3. 将结果转化为可以执行的人际协作。

## 安装

使用 Skills CLI：

```bash
npx skills add hunterhigh/cognitive-skills
```

手动安装时，将 [`skills/`](skills/) 下任意一个完整目录复制到个人或项目级 Skills 目录。

## 使用

```text
使用 $first-principles-dialogue，找出这个命题中的原子事实和隐含假设。
使用 $situated-decision，根据证据、利益、不确定性和可能发生的变化检验这个方案。
使用 $work-alignment-advisor，把这个判断转化为面向相关人员的清晰消息和下一步。
```

## 设计原则

- **推理先于表达。** 在优化结论如何呈现前，先暴露它所依赖的假设和证据。
- **语境会改变有效性。** 决策需要放进实际运行环境中检验，而不只是作为抽象论证评价。
- **人际协作是独立层次。** 沟通和责任边界属于执行系统的一部分，不是事后的包装。
- **保留不确定性。** 明确未知项、可逆行动以及可能改变决定的新证据。
- **软件包相互独立。** 每个 Skill 都有自己的入口，可以单独安装。

## 仓库结构

```text
skills/
├── first-principles-dialogue/
├── situated-decision/
└── work-alignment-advisor/
```

## 验证

使用官方 Skill 验证器检查单个 Skill：

```bash
python /path/to/skill-creator/scripts/quick_validate.py skills/<skill-name>
```
