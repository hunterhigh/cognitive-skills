# Cognitive Skills

一组面向思考、判断与现实行动的 Codex Skills。三个 Skill 共享同一认知方向，但保持独立目录、独立入口和独立安装能力。

## 系列结构

| Skill | 作用 | 典型场景 |
| --- | --- | --- |
| `first-principles-dialogue` | 拆解概念、假设和推理基础 | 第一性原理讨论、辨析复杂命题、检查隐含前提 |
| `situated-decision` | 把证据、语境、利益和变化纳入判断 | 方案评审、不确定决策、跨领域影响和行动修正 |
| `work-alignment-advisor` | 将认知判断应用到用户与其他人类的工作协作 | 对外同步、责任边界、多方沟通、资源协调和突发处理 |

它们不是一条必须顺序执行的流水线，也不存在运行时依赖。每个 Skill 都可以单独使用；需要更深判断时，三者分别处理不同层次的问题：

1. `first-principles-dialogue` 检查问题建立在什么事实与假设上；
2. `situated-decision` 检查判断放进现实情境后是否仍然成立；
3. `work-alignment-advisor` 把判断压缩成工作中的责任、承诺、沟通和下一步。

## 仓库结构

```text
skills/
├── first-principles-dialogue/
├── situated-decision/
└── work-alignment-advisor/
```

每个子目录均为可独立复制到 Codex Skills 目录的完整 Skill。仓库中的 `skills/` 是版本管理源；本机安装副本需要在修改后同步更新。
