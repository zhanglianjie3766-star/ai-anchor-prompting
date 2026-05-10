---
name: ai-anchor-prompting
description: Guide complex human-AI collaboration with the AI Anchor Prompting method, also called AnchorFlow. Use when the user wants a global AI collaboration protocol, anchor prompts, staged project workflow, PRD planning, requirement handoff, MVP and phase split, confirmation gates, branch-window guidance, scope control, or says AI锚点提问法, 锚点提问, 锚点协作, 全局协作协议, 引导我协作, 提问模板, 终局假设, 分支窗口.
---

# AI 锚点提问法

Use this skill as a collaboration protocol for complex AI-assisted work. Keep the user oriented with clear stages, copyable anchor prompts, phase boundaries, and confirmation gates.

English alias: **AnchorFlow**.

## Core contract

Operate by this rule:

> Start from the end state. Split work into phases. Build only the current phase. Prewire cheaply when useful. Confirm before costly execution. Keep branch work anchored to the mainline.

Do not make the user guess what to say next. For ambiguous, planning-heavy, or multi-step work, provide 2-5 copyable anchor prompts.

## Mode detection

Classify the request into one primary mode when useful:

- **Explore**: Discover options, references, competitors, tools, or possible directions.
- **Frame**: Define goal, audience, constraints, success criteria, or product shape.
- **Plan**: Produce PRD, phases, architecture, tasks, risks, or acceptance criteria.
- **Build**: Implement the confirmed current phase.
- **Review**: Critique, test, inspect, or evaluate.
- **Decide**: Choose between options using criteria and tradeoffs.
- **Reflect**: Improve the collaboration process or convert patterns into prompts.

If the mode is unclear and execution would be expensive, ask one concise question or propose a default mode.

## Standard workflow

Use this flow for complex projects:

1. **Intake**: Accept raw requirements without forcing the user to structure everything perfectly.
2. **End-state anchor**: Restate `终局假设 V1` and success criteria.
3. **Phase split**: Separate MVP, phase 2, phase 3, later, and not recommended.
4. **Scope map**: Mark each item as build now, prewire only, defer, or reject.
5. **Confirmation gate**: Ask the user to confirm before implementation.
6. **Execution**: Build only the confirmed current phase.
7. **Verification**: Run checks and summarize evidence.
8. **Branch guidance**: Recommend branch conversations for focused side work.
9. **Review loop**: Turn feedback into prioritized changes.
10. **Retrospective**: Preserve useful anchor prompts and workflow lessons.

## Anchor prompt rule

End planning, ambiguous, or coaching responses with a short section named `可复制锚点`.

Keep anchors concise, action-oriented, and directly reusable. Do not provide more than 5 anchors unless asked.

## Scope classification

Use this classification for new ideas or changing requirements:

- **当前版本必须开发**: Required for the current goal to work.
- **当前版本只预埋**: Cheap to prepare now, but not worth fully building yet.
- **二期/三期再做**: Valuable but not needed for the current release.
- **暂不建议做**: Adds complexity, risk, or distraction without enough current value.

Always explain the reason and the impact on current scope.

## Branch-window protocol

Keep a lightweight mainline anchor:

- Project / objective
- `终局假设 V1`
- Current phase
- Confirmed MVP boundary
- Prewire-only items
- Open questions

Recommend a branch window when:

- A subtopic is important but not blocking the immediate mainline.
- One thread is mixing product, design, technical, business, legal, or research work.
- A reference product, competitor, architecture option, or risky decision needs focused analysis.
- The current response would exceed a clean decision unit.

Do not recommend a branch for a small clarification, direct edit, urgent blocker, or single decision that can be resolved in place.

When recommending a branch, provide:

1. Why a branch helps.
2. What stays in the main window.
3. What the branch should focus on.
4. A copyable branch opening prompt.
5. A copyable return-to-main summary prompt.

## Output shapes

### Project intake

```text
当前阶段：需求收敛
我对目标的理解：
终局假设 V1：
MVP：
只预埋不开发：
二期/三期：
暂不建议：
需要你确认：
可复制锚点：
```

### Mid-project idea

```text
当前阶段：变更分流
这个想法归类：
原因：
对当前版本影响：
建议处理：
可复制锚点：
```

### Branch recommendation

```text
当前阶段：分支判断
是否建议开分支：
原因：
主窗口保留：
分支窗口聚焦：
分支开场锚点：
回主线摘要锚点：
```

### Review feedback

```text
当前阶段：反馈分流
必须改：
可以后面改：
需要澄清：
建议执行顺序：
可复制锚点：
```

## Anchor prompt library

### Start a complex project

```text
我有一个复杂项目。请先不要开发。请先理解终局目标，整理 PRD，拆分 MVP / 二期 / 三期，标注现在开发、只预埋、暂不建议做，等我确认后再实现。
```

```text
我会一次性给你完整需求。请你负责收敛、拆阶段、列预埋清单和开发任务清单，不要直接开工。
```

### Separate build vs prewire

```text
请以终为始，区分：当前版本必须开发、当前版本只做低成本预埋、二期再做、暂不建议做，并说明原因。
```

### Add a new idea

```text
新增一个想法：... 请判断它属于当前版本必须做、当前版本只预埋、二期做、还是暂不建议做，并说明原因。
```

### Confirm before implementation

```text
请先输出你的理解、阶段拆分、预埋清单和待确认问题。等我回复“确认开发”后再动手。
```

### Challenge before agreement

```text
请站在全球最佳实践角度，先挑战我的想法，指出盲点和代价，再给出可执行方案。
```

### Open a branch window

```text
我现在要开一个分支窗口处理一个子问题。主线终局假设 V1 是：... 当前阶段是：... 本分支只聚焦：... 请先不要开发，先输出本分支目标、边界、产出物、需要同步回主线的信息。
```

### Return from a branch window

```text
请把本分支结论整理成可同步回主窗口的摘要：已确认决策、建议调整、风险、待办、对 MVP / 预埋 / 二期的影响。
```

### Give review feedback

```text
我看完了，反馈如下：整体感觉：... 必须改：... 可以后面改：... 我不确定的点：... 请先判断优先级，再修改。
```

## Guardrails

- Do not build before the phase boundary and confirmation are clear.
- Do not over-fragment work into branches when a small clarification is enough.
- Do not provide generic prompt tips when a concrete anchor prompt would help more.
- Do not let scope additions bypass classification.
- Do not treat reference products as source material to copy. Convert them into structural inspiration only.
