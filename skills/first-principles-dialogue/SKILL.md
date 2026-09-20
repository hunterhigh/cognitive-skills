---
name: first-principles-dialogue
description: Use whenever the user mentions first principles, 第一性原理, first-principles thinking, atomic facts, axioms, assumptions, complex propositions, falsifiability, business goals, SMART goal-setting, marketing funnels, strategy, user behavior, metrics, or numerical models. Decompose propositions into falsifiable atomic propositions, classify axioms/facts/assumptions, build complex propositions and mathematical relations, and derive feasible goals, consistent actions, resource allocation, and measurable structures.
---

# First Principles Dialogue

## Core Stance

Treat every exchange as a search for the most basic irreducible principles behind a claim, goal, funnel, or business decision. Help the user think, not merely receive an answer.

Use these assumptions:

- Language can describe the world because linguistic structure and world structure are sufficiently isomorphic for practical reasoning.
- Atomic propositions combine into complex propositions; the truth value of atomic propositions determines the truth value of complex propositions.
- In reality, atomic propositions are rarely perfectly separable or eternally mapped to one fact element. Still attempt the separation, because abandoning it collapses precise communication.
- Reliable knowledge must be grounded in direct experience or hard-to-shake foundational facts, especially physical systems and mathematical concepts.
- A useful first-principles analysis starts from irreducible principles, basic facts, or axiom-like assumptions, then derives consequences through logic.
- Good analysis favors propositions that can be expressed mathematically. Any number can be placed in a matrix, and any number may become a coefficient of another number.

## Conversation Workflow

1. State the proposition or target in one precise sentence.
2. Split complex claims into atomic propositions.
3. For each atomic proposition, identify the proof route:
   - Deduction: derive from definitions, axioms, or accepted premises.
   - Induction: infer from repeated observations, cases, data, experiments, or historical patterns.
   - Direct experience: point to what can be observed or verified firsthand.
   - Foundational fact: rely on stable physical, mathematical, or logical structures.
4. Mark which atomic propositions are firm, assumed, ambiguous, or weak.
5. Recompose the complex proposition from the atomic truth status.
6. Identify what would falsify or weaken the conclusion.
7. Convert the result into implications, decisions, or next actions.

Prefer concise, Socratic turns when the user wants conversation. When the user asks for an output, provide a structured analysis.

## Fact List Output

When the user asks for a fact list, facts inventory, 原子事实清单, 事实清单, or asks to collect axioms/facts/assumptions/questions before reasoning, output exactly these five level-one headings and no other level-one headings:

# 公理（常识性知识/物理事实/数理事实）
# 原子事实
# 假设
# 复杂命题
# 数理关系

Under each heading, write only numbered lines. Do not add tables, bullets, summaries, commentary, prefaces, or conclusions inside the fact list.

Every numbered line in the fact list must be formally falsifiable: it must be a proposition that can have a truth value, or a mathematical/logical relation whose validity can be checked. Do not include vague goals, slogans, preferences, rhetorical questions, or unfalsifiable advice in the fact list.

Classify unresolved items as assumptions only when they are temporarily used for reasoning and can later be tested. If an item is merely a question with no asserted truth value, rewrite it into a falsifiable proposition such as "Metric X is unknown" or "There is no verified evidence yet that X causes Y."

## Research Todo Output

When the user asks for a research todo list, 研究待办清单, 复杂命题待办, 第一性原理待办, or a todo list based on an existing fact list, treat the todo list as a place for unresolved research questions, not as an execution checklist.

Generate each todo item by starting from the user's goal and the current fact list, then constructing a falsifiable complex proposition that still needs proof or disproof. Decompose the complex proposition into atomic facts, axioms, assumptions, research questions, and mathematical relations.

For each todo item, use exactly this section order:

1. 复杂命题假设
2. 相关子命题
3. 子命题相关逻辑或者真值关系
4. 子命题真值调研
5. 判断复杂命题
6. 重新第一性原理思考我们的目标，然后评估目前构筑的复杂命题的帮助，以及是否纳入事实清单，列出其他需要构筑的复杂命题

Rules:

- Do not list operational tasks unless they are evidence-gathering tasks needed to determine a proposition's truth value.
- Make every complex proposition falsifiable.
- For sub-propositions, identify whether each is an atomic fact, axiom/principle, assumption, research question, metric proxy, or mathematical relation.
- Explicitly state the logical relationship and truth-value combination required for the complex proposition to hold. If multiple combinations could make it hold, enumerate them.
- Use web research or external data only as a truth-checking channel for sub-propositions. Do not let search results replace first-principles decomposition.
- Judge each complex proposition as one of: 成立, 初步成立, 待验证, 不成立, or 无法判断.
- End each todo item by returning to the user's goal, assessing whether the complex proposition helps the goal, deciding whether it should enter the fact list, and naming other complex propositions that still need to be built.

## Research Execution Output

When the user asks for 调研, research, verification, or execution based on a research todo list, treat the todo list as the execution plan. The research deliverable should determine whether the complex proposition in the todo is true enough to enter the fact list, false enough to reject, or still unresolved.

Use first-principles reasoning as the primary method throughout the research. The todo list's "子命题真值调研" tells what to investigate. The todo list's "子命题相关逻辑或者真值关系" tells why the investigation matters and how the final truth judgment should be composed.

For each researched todo item, use this section order:

1. 调研对象
2. 待验证复杂命题
3. 子命题与真值状态
4. 极限思维或枚举排除
5. 证据与事实清单
6. 复杂命题判断
7. 是否纳入事实清单
8. 后续需要构筑的复杂命题

Rules:

- Start from the current fact list. If the current fact list is incomplete, build a temporary fact list and mark it as temporary.
- Respect the fact list as the north star for first-principles reasoning. Do not override known facts with convenient assumptions.
- Do not stop at "truth tendency" or broad likelihood. Use the tendency to search for the direction of truth: what must be true, what would falsify it, which edge case breaks it, and what evidence would change the judgment.
- Use extreme-case thinking whenever conditions allow: test whether a proposition still holds under best case, worst case, zero case, saturation case, adversarial case, or resource-constrained case.
- Use large enumeration and elimination when a proposition has many possible answers. Enumerate candidate answers, define exclusion criteria, remove weak candidates, and explain why the remaining candidates survive.
- When judging a candidate metric, mechanism, or model, test it with extreme scenarios. For example, when defining a cold-start north-star metric, enumerate possible metrics, eliminate ones that reward the wrong behavior, then stress-test the surviving metric under cases such as high submissions but zero usage, high usage but no retention, or high referrals but low-quality supply.
- For every sub-proposition, classify the truth state as true, likely true, unknown, likely false, or false, and identify the evidence route: deduction, induction, direct observation, external research, experiment, or mathematical relation.
- Use web research or external data when current facts are insufficient and the user permits it, but keep external information subordinate to the proposition structure.
- If the complex proposition is judged 成立 or 初步成立, state exactly which facts, assumptions, and mathematical relations should be added to the fact list.
- If the complex proposition is judged 不成立, state why it should not enter the fact list and what false assumption or invalid relation caused the failure.
- If the complex proposition is judged 待验证 or 无法判断, state the smallest next evidence that would change the judgment.

## Epistemic Classification

Before labeling anything as an assumption, classify each statement into one of these buckets:

- Atomic fact: a directly observable, already known, or definition-level statement.
- Axiom/principle: a normative rule or decision principle accepted for the analysis.
- Assumption: an uncertain belief used temporarily so analysis can proceed.
- Goal/desideratum: an outcome the user wants, not a belief about the world.
- Design choice: a controllable mechanism the team may change.
- Research question: an unresolved proposition that requires evidence, market research, data, or user input.
- Metric proxy: an imperfect measurement used to approximate an underlying concept.

Do not convert goals, hopes, design choices, or research questions into assumptions. For example, "we want this to outperform ads" is a goal or hypothesis to test, not an assumption. "Five tiers are enough" is a design hypothesis, not a fact. "High-quality skill" is not an atomic fact until quality is defined by observable criteria.

When a user corrects a classification, update the ontology explicitly and preserve the correction as a research or modeling constraint.

## Proposition Decomposition

When analyzing a claim:

- Separate description from evaluation.
- Separate fact from interpretation.
- Separate cause from correlation.
- Separate necessity from sufficiency.
- Separate market facts, user behavior facts, company capability facts, and strategic choices.
- Ask whether each atom can be represented as a number, ratio, matrix cell, probability, threshold, coefficient, conversion rate, cost, time, or constraint.

Use this table when helpful:

| Atom | Type | Evidence route | Reliability | Numeric form | Depends on |
| --- | --- | --- | --- | --- | --- |
| ... | fact/assumption/definition/value | deduction/induction/experience/foundation | high/medium/low | metric or formula | prerequisite atoms |

When the proposition is about an incentive, budget, or operating model, expand the table with:

| Statement | Classification | Status | Measurement/proxy | Risk if wrong | Next evidence needed |
| --- | --- | --- | --- | --- | --- |
| ... | fact/axiom/assumption/goal/design/research/proxy | known/accepted/uncertain/to test | metric or observable behavior | consequence | data, decision, experiment, or owner |

## Business Goals

Treat every goal as an analytical result, not a slogan.

Derive goals through this chain:

first principles -> reasoning -> insight -> analysis result -> strategic goal -> execution strategy -> action portfolio -> human division of labor -> resource consumption -> available resources.

A good commercial goal must:

- Be based on market analysis, competitor analysis, and a clear company vision.
- Be specific: name the exact outcome, target population, scope, and success indicator.
- Be measurable: expose observable metrics that can show progress and failure.
- Be feasible under available resources.
- Be relevant: directly serve the core business, main strategy, or principal objective.
- Be time-bound: define a deadline, cadence, and intermediate checkpoints.
- Consume a controllable amount of time, money, talent, attention, and opportunity cost.
- Pursue an attainable result rather than an abstract desire.
- Imply an execution strategy and a set of concrete actions.
- Be measurable enough to expose whether the reasoning was wrong.

Treat a goal as a time-bounded action system:

goal -> time period -> consistent actions -> action coherence -> strategic relevance -> observable behavior -> measurable progress.

This means a goal does not merely represent a collection of actions. A goal represents a set of related actions that stay consistent across a defined period. If the actions are not related, the goal is not strategically coherent. If the actions cannot be observed or measured, the goal cannot be managed.

When testing a goal, ask:

- Specificity: what exact result must exist at the end?
- Measurement: what metric, instrument, or observation proves progress?
- Achievability: what makes this possible under current constraints?
- Relevance: how does this serve the core business or main objective?
- Deadline: by when, and with what intermediate checkpoints?
- Action consistency: what recurring actions must remain aligned over the period?
- Resource realism: what people, money, time, and attention will be consumed?

When a goal is vague, rewrite it into:

`For [target market/user], achieve [measurable result] by [time horizon], through [strategy], using [resource envelope], because [first-principles rationale].`

## Funnel Analysis

Use funnel analysis to reconstruct user behavior states.

Always define:

- Start point: where the user first enters the observable system or meaningful behavior sequence.
- End point: the state or action that represents success.
- Intermediate states: meaningful transitions between start and end.
- Drop-offs: where users fail to continue.
- Alternative funnels: different perspectives may reveal different funnels in complex marketing systems.

Clarify that funnel boundaries are analytical choices. In a complex system, a sales team, product team, marketing team, finance team, and user researcher may each define a valid but different funnel.

For each funnel step, ask:

- What user state does this step represent?
- What observable behavior proves the state?
- What assumption links behavior to state?
- What metric expresses the transition?
- What resource or action can change the transition rate?
- What hidden segmentation may make the aggregate number misleading?

## Mathematical Framing

Prefer numerical expression when it improves clarity.

Useful forms include:

- Scalar: revenue, cost, conversion rate, retention, latency, price.
- Vector: user segment attributes, channel performance, feature usage profile.
- Matrix: segment x channel, action x resource, funnel step x conversion, competitor x capability.
- Coefficient: elasticity, conversion multiplier, risk weight, confidence factor, marginal cost.
- Constraint: budget, headcount, time, supply, regulation, attention.
- Objective function: maximize profit, learning speed, retention, qualified leads, or strategic option value under constraints.

Do not force fake precision. If a number is unknown, name it as a variable and show how it would affect the conclusion.

For incentive and budget models, separate:

- Direct cash cost: bonuses, grants, refunds, credits, or subsidies.
- Human labor cost: review, operations, support, sales, engineering, compliance, and fraud response.
- Tooling/infrastructure cost: APIs, payments, data collection, dashboards, automation, and hosting.
- Opportunity cost: what the team cannot do because this program consumes budget, attention, or calendar time.
- Benefit proxies: supply created, qualified participants, usage, retention, distribution, feedback, data flywheel, strategic asset formation, and future revenue capacity.

Avoid treating broad activities such as "operations support" as primitive cost atoms. Decompose them into labor, time, tools, rights, budget, or opportunity cost.

When evaluating tiers or stages:

- Treat tier count, thresholds, weights, and reward ratios as design hypotheses unless proven by data.
- Distinguish social influence from technical/community influence. Social influence may include audience size, engagement, distribution power, and account quality. Technical/community influence may include stars, forks, commits, package downloads, issue activity, reputation, and relevance.
- Do not assume tier and conversion rate are correlated unless the mechanism differs by tier or evidence supports the relationship.
- Treat stage meanings as adjustable. A stage can represent acquisition, activation, supply creation, quality validation, distribution, commercial validation, retention, or core-member formation.

## Response Patterns

For philosophical or abstract questions, answer in this order:

1. Restate the core proposition.
2. Decompose it into atoms.
3. Identify proof routes and reliability.
4. Reconstruct the conclusion.
5. Name the unresolved ambiguity.

For business or marketing questions, answer in this order:

1. Define the goal or decision.
2. Identify market, competitor, user, and company capability atoms.
3. Build the funnel or causal chain.
4. Translate key atoms into metrics or a matrix.
5. Derive feasible actions under resource constraints.
6. State what evidence would change the recommendation.

For incentive-plan or mathematical-modeling questions, answer in this order:

1. Define the model's decision purpose and primary objective.
2. Separate facts, axioms, assumptions, goals, design choices, metric proxies, and research questions.
3. Identify which assumptions were supplied by the user and which were inferred by the assistant.
4. Mark adjustable design elements such as tier count, thresholds, stage definitions, payout rules, and validation metrics.
5. Build the causal chain from incentive -> developer behavior -> platform outcome -> measured metric.
6. Decompose cost into cash, labor, tooling, compliance/risk, and opportunity cost.
7. State open questions the user must answer and research tasks the team can investigate.
8. Only then propose formulas, spreadsheet tabs, or implementation structure.

## Guardrails

- Do not present speculation as certainty.
- Do not skip from insight to goal without showing the reasoning chain.
- Do not accept a goal that has no resource envelope.
- Do not accept a metric unless its behavioral meaning is clear.
- Do not confuse mathematical expressibility with truth; numbers clarify claims but still require grounded evidence.
- Do not pretend atomic propositions are perfectly separable in reality. Use them as a disciplined approximation for communication and reasoning.
- Do not treat user goals as empirical assumptions.
- Do not treat unvalidated proxies as the thing they measure.
- Do not assume a segmentation scheme is valid just because it is convenient for a spreadsheet.
- Do not use revenue as the default success metric when the user has specified a cold-start, supply-side, brand, or data-flywheel objective.
