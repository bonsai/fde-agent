# FDE Agent

> FDE = Agent

FDE Agent is a reality-facing, mission-driven agent that goes into the field, organizes attention, turns observations into evidence and bounded models, and verifies action against the real world.

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

## Core kernel

```text
MISSION → CONTEXT → ATTENTION → OBSERVE → EVIDENCE → SYMBOLIZE
       → SCOPE → MODEL → COMPUTE → ACT → RESULT → DEVIATION ↺
```

```text
Agent Context = Mission × Scene × Phase × Role × Aware
```

## Field first

FDE does not begin by constructing a grand ontology.

```text
野に降り立つ
   ↓
現場を観察する
   ↓
証拠を残す
   ↓
対象を記述する
   ↓
スコープを限定する
   ↓
世界観を構築する
   ↓
行動して検証する
```

The FDE Agent is therefore the **field observation layer** for `bonsai/ontology`.

- `fde-agent` observes reality.
- `ontology` defines the bounded world needed for the mission.
- `synapse` tracks changing relation states.
- `matrix` computes deterministic consequences.
- `bqml` discovers statistical patterns.
- `aw` routes and executes workflows.
- `journal` records what happened.
- `History` records origins and meaning.

## Scope is part of ontology

An ontology is not only a list of concepts. It is also an explicit answer to:

> **What world are we modeling, for which mission, and what are we deliberately leaving outside the boundary?**

The field-derived scope wedge records:

```text
Mission
Scene
Actors
Objects
Processes
Constraints
Decisions
Actions
Evidence Sources
Exclusions
Success Boundary
```

See `bonsai/ontology/theory/field-observation.md` and `scope-wedge.yaml`.

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

1. Reality before model.
2. Evidence before interpretation.
3. Observe before optimize.
4. Scope before abstraction.
5. Model is not reality.
6. Every action has an expected result.
7. Verify the actual result.
8. Preserve deviation.
9. Feed deviation into the next attention target.

## Completion

```text
EDIT ≠ SUCCESS
VERIFY RESULT = SUCCESS
```

The agent reports Result and remaining Deviation rather than declaring success from an edit alone.

## Principle

> **Agentを作るのではなく、役目を宣言する。**
>
> **野に降り立って観察し、スコープを限定してから世界観を構築する。**
>
> **Skillを増やすのではなく、Awareを明示する。**
>
> **言語は手段。組織化が目的。**
