<div align="right">

**English** | [简体中文](README.zh-CN.md)

</div>

# Cognitive Skills

**A collection of agent skills for reasoning from fundamentals, making context-aware decisions, and turning judgment into workable human alignment.**

Cognitive Skills is built around a simple distinction: a sound premise, a sound decision, and a sound workplace action are related—but they are not the same problem. The repository keeps those responsibilities separate and composable.

## Skills

| Skill | Responsibility | Use it when |
| --- | --- | --- |
| [`first-principles-dialogue`](skills/first-principles-dialogue/SKILL.md) | Decompose claims into facts, assumptions, definitions, and inference | A concept or complex proposition needs to be examined from first principles. |
| [`situated-decision`](skills/situated-decision/SKILL.md) | Test a judgment against evidence, context, incentives, uncertainty, and change | A locally plausible solution may fail in the wider real-world system. |
| [`work-alignment-advisor`](skills/work-alignment-advisor/SKILL.md) | Convert judgment into clear commitments, boundaries, communication, and next steps with other people | The challenge is alignment with a manager, colleague, client, or partner. |

The skills do not form a required pipeline. Use one on its own, or combine them when a decision needs deeper examination:

1. establish what the claim is built on;
2. test whether it remains valid in context;
3. translate the result into workable human coordination.

## Install

Using the Skills CLI:

```bash
npx skills add hunterhigh/cognitive-skills
```

For manual installation, copy any complete directory under [`skills/`](skills/) into your personal or project-level Skills directory.

## Use

```text
Use $first-principles-dialogue to identify the atomic facts and hidden assumptions in this claim.
Use $situated-decision to test this proposal against evidence, incentives, uncertainty, and likely change.
Use $work-alignment-advisor to turn this judgment into a clear message and next step for the people involved.
```

## Design principles

- **Reasoning before rhetoric.** The skills expose assumptions and evidence before optimizing how a conclusion sounds.
- **Context changes validity.** A decision is evaluated inside its operating environment, not only as an abstract argument.
- **Human coordination is its own layer.** Communication and responsibility boundaries are treated as part of execution, not as an afterthought.
- **Uncertainty remains visible.** Unknowns, reversible actions, and evidence that could change the decision are made explicit.
- **Independent packages.** Each skill has its own entry point and can be installed without the others.

## Repository structure

```text
skills/
├── first-principles-dialogue/
├── situated-decision/
└── work-alignment-advisor/
```

## Validation

Validate an individual skill with the official skill validator:

```bash
python /path/to/skill-creator/scripts/quick_validate.py skills/<skill-name>
```
