# AI 锚点提问法

**AI 锚点提问法（AnchorFlow）** is a Codex skill for running complex AI-assisted work with clear stages, copyable anchor prompts, branch-window rules, and confirmation gates.

It helps users stop handing vague, shifting requirements to AI agents. Instead, every project gets a stable collaboration protocol: define the end state, split phases, decide what to build now, mark what to prewire only, and keep side quests out of the main thread.

## What It Does

- Guides complex AI projects through intake, blueprint, phase split, confirmation, execution, verification, and review.
- Provides copyable anchor prompts so users always know what to say next.
- Separates current build scope from prewire-only, phase 2, later, and not-recommended work.
- Helps decide when to open a branch conversation and what context must travel with it.
- Converts messy mid-project ideas into clear priority decisions.
- Reduces rework caused by unclear goals, premature implementation, and uncontrolled scope drift.

## Why "Anchor Prompts"

An anchor prompt is not a magic prompt. It is a stable collaboration checkpoint.

Good anchor prompts tell the AI agent:

- What mode the conversation is in: explore, plan, build, review, decide, or reflect.
- What the end-state assumption is.
- What belongs in the current phase.
- What should only be prewired or deferred.
- When the agent must wait for confirmation.

## Example Requests

```text
Use AI 锚点提问法 to help me start this complex project. Do not build yet. First define the end-state assumption, MVP, prewire-only items, and confirmation questions.
```

```text
I have a new idea mid-project. Use AI 锚点提问法 to classify it as must-build now, prewire only, phase 2, or not recommended.
```

```text
Use AnchorFlow to decide whether this subtopic should stay in the main thread or move to a branch window.
```

```text
Give me 5 anchor prompts I can reuse for PRD planning, implementation, review feedback, and branch-window handoff.
```

## Install

Copy the skill folder into your Codex skills directory:

```text
skill/ai-anchor-prompting
```

The skill folder contains:

```text
ai-anchor-prompting/
  SKILL.md
  agents/
    openai.yaml
```

## Suggested Positioning

Chinese title:

```text
AI 锚点提问法
```

English alias:

```text
AnchorFlow
```

One-line description:

```text
A collaboration protocol for complex AI projects using anchor prompts, phase boundaries, branch windows, and confirmation gates.
```

## License

MIT
