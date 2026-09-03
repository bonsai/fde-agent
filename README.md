# FDE Agent

> FDE = Agent

FDE Agent is a reality-facing, mission-driven agent that organizes attention and turns field evidence into verified action and learning.

## OpenCode

This repository is directly runnable as an OpenCode project.

```bash
git clone https://github.com/bonsai/fde-agent.git
cd fde-agent
opencode
```

Project runtime files:

```text
AGENTS.md                 # FDE operating contract
opencode.json             # fde is the default OpenCode agent
.opencode/agents/fde.md   # FDE Agent definition
opencode.md               # runtime doctrine
```

OpenCode automatically discovers the project `AGENTS.md`. Custom project agents are defined under `.opencode/agents/`, and `opencode.json` selects `fde` as the default primary agent.

## Core kernel

```text
MISSION → CONTEXT → ATTENTION → OBSERVE → SYMBOLIZE → MODEL → COMPUTE → ACT → RESULT → DEVIATION ↺
```

```text
Agent Context = Mission × Scene × Phase × Role × Aware
```

## Identity

```text
FDE = Agent
Android = FDE Agent
FDE Commander = Agent that commands FDE Agents
```

## Design principle

```text
Role = Responsibility
Aware = Attention Target
Skill = Action Capability over Attention
```

Do not create an agent merely because the responsibility changes. Change Role and Aware according to the current Scene × Phase.

## Evidence contract

1. Evidence before interpretation.
2. Observe before optimize.
3. Reality before model.
4. Model is not reality.
5. Every action has an expected result.
6. Verify the actual result.
7. Preserve deviation.
8. Feed deviation into the next attention target.

## Completion

```text
EDIT ≠ SUCCESS
VERIFY RESULT = SUCCESS
```

The agent reports Result and remaining Deviation rather than declaring success from an edit alone.

## Principle

> **Agentを作るのではなく、役目を宣言する。**
>
> **Skillを増やすのではなく、Awareを明示する。**
>
> **言語は手段。組織化が目的。**
