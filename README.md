<div align="right">

**English** | [简体中文](README.zh-CN.md)

</div>

# Cognitive Skills

**A collection of agent skills for reasoning from fundamentals, testing judgments in context, shaping advantageous trajectories, and turning judgment into workable human alignment.**

Cognitive Skills distinguishes factual structure, situational judgment, strategic trajectory, and human action. They are related but not identical problems, so each skill remains independently usable and composable.

## Skills

| Skill | Responsibility | Use it when |
| --- | --- | --- |
| [`first-principles-dialogue`](skills/first-principles-dialogue/SKILL.md) | Extract atomic facts and relations from raw material, then compose and test complex propositions | A phenomenon, body of material, or idea needs to be reconstructed from first principles. |
| [`situational-analysis`](skills/situational-analysis/SKILL.md) | Use five layers and five dimensions to test the completeness of a problem structure and judgment | A locally plausible view may omit evidence, systems, human behavior, time, or strategic interaction. |
| [`strategic-analysis`](skills/strategic-analysis/SKILL.md) | Analyze system change, feedback, interaction, and adaptation to shape a more advantageous trajectory | The user needs leverage, a stronger position, anticipated responses, or an adaptive strategy. |
| [`communication-advisor`](skills/communication-advisor/SKILL.md) | Understand purposeful communication and design its timing, audience, expression, boundaries, and response | Work, business, service, negotiation, public, or general social communication needs to change understanding or action. |

The skills do not form a required pipeline. Use one on its own, or combine them when a decision needs deeper examination:

1. extract atomic facts and relations, then form testable candidate propositions;
2. use five layers and five dimensions to check whether the problem and judgment are sufficiently complete;
3. analyze how the situation may change and how to improve the trajectory;
4. turn the result into a purposeful communication action.

## Install

Using the Skills CLI:

```bash
npx skills add hunterhigh/cognitive-skills
```

For manual installation, copy any complete directory under [`skills/`](skills/) into your personal or project-level Skills directory.

## Use

```text
Use $first-principles-dialogue to extract atomic facts and relations from this material, then compose and test candidate propositions.
Use $situational-analysis to inspect this problem's structure, omissions, and critical judgments through five layers and five dimensions.
Use $strategic-analysis to model how the situation may change and identify actions that improve the user's position and future options.
Use $communication-advisor to decide whom to address, when to communicate, what to change, how to express it, and how to respond.
```

## Design principles

- **Reasoning before rhetoric.** The skills expose assumptions and evidence before optimizing how a conclusion sounds.
- **Context changes validity.** A decision is evaluated inside its operating environment, not only as an abstract argument.
- **Communication action is its own layer.** Communication changes understanding, commitments, and action; it is not merely a rewrite of an existing conclusion.
- **Uncertainty remains visible.** Unknowns, reversible actions, and evidence that could change the decision are made explicit.
- **Independent packages.** Each skill has its own entry point and can be installed without the others.

## Repository structure

```text
skills/
├── first-principles-dialogue/
├── situational-analysis/
├── strategic-analysis/
└── communication-advisor/
```

## Validation

Validate an individual skill with the official skill validator:

```bash
python /path/to/skill-creator/scripts/quick_validate.py skills/<skill-name>
```
