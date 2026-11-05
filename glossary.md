# Celestelin Glossary

> Terms coined or defined in the research of Aria Chen, Celestelin Research, Calgary, Canada. Each entry gives a one-sentence definition, a fuller explanation, and where the term comes from.

HTML version: https://celestelin.com/glossary.html · Contact: aria@celestelin.com

## The program

### Celestelin

An independent research ecosystem of about 130,000 lines of running code, built and operated by Aria Chen and continuously deployed since April 2025, studying how long-running human–AI systems stay trustworthy.

Each research topic in Celestelin is a problem the running system met first; the papers came after the system. Six systems (Workshop, CelestelinAgent, EXO, Home, Multi-Agent Workshop, SoulNest) share two substrates: an identity layer (PersonaCore) and a memory engine (MemoryCore).

中文：一个约 13 万行、2025 年 4 月起持续运行的研究生态，由 Aria Chen一人搭建和运营，研究长期运行的人机系统怎样保持可信。先有系统，后有论文。

Source: [Research landscape](https://celestelin.com/research-landscape.html); [celestelin.ai](https://celestelin.ai)

### Research iceberg (above, at and below the waterline)

The map of the Celestelin program: human–AI interaction above the waterline, language at the waterline, and the mechanisms that keep a long-running agent trustworthy below it.

The sea is the interaction field that grows between a person and an AI. Below the water, memory, trajectory, active work, runtime state and values sit side by side and together form the agent's longitudinal state. PersonaCore, the identity anchor, sits beneath every architecture. Each paper takes responsibility for one property a long-running human–AI system has to keep.

中文：水面上是交互，水线上是语言，水面下是可信。海水是人和 AI 一起长出来的交互场；每一篇论文替长期运行的人机系统守住一样东西。

Source: [Research landscape](https://celestelin.com/research-landscape.html)

### Longitudinal state

Everything a long-running agent carries across time that has to stay trustworthy: memory, trajectory, active work, runtime state and values, held side by side.

In the Celestelin landscape each part of the longitudinal state has its own mechanism: memory (SSR and MemoryCore), trajectory (Awareness Mirror), active work (ThreadPulse), runtime state (G-Value Dynamics) and values (person-centered safety).

中文：长期运行的 agent 随时间带着走、又必须保持可信的一切：记忆、轨迹、手头的工作、运行时状态和价值。

Source: [Research landscape](https://celestelin.com/research-landscape.html)

## The interaction field

### Interaction field

The evolving dynamic structure jointly formed through interaction, shaping the conditions for what can happen next. Both parties make it; it holds both of them.

The same words carry different force in different fields: “Go ahead” can mean trust after fluent collaboration, resignation after repairs went nowhere, or challenge after trust wore thin. The field is built by everything that came before. The interaction field was introduced as a unit of analysis for long-term human–AI relations beyond trust and satisfaction.

中文：交互双方共同形成、持续演化的动力结构，它塑造着接下来互动发生的条件。两个人一起造出它，它也同时托着两个人。

Source: [Interaction Field Dynamics](https://celestelin.com/demo/interaction-field.html); [Beyond Trust and Satisfaction (SSRN working paper)](https://celestelin.com/papers.html)

### Interaction Field Dynamics (IFD)

A framework that makes long human–AI interaction measurable by decomposing it into four observable variables: State, Action, Flow and Readout.

State is where the interaction is right now (16 numbers: four shared dimensions, three held by each side, and six interactional positions). Action is what a turn does to that State. Flow is the shape of the path the steps trace together: coupled, drifting, swinging, stuck, recovering, breaking, resonating or waking up again. Readout is what really happened next, recorded on a separate evidence channel, so the field never grades itself. In two independent sets, the 16-number State predicts whether the next speaker will correct the turn at AUROC .731 and .710, against .463 and .448 for the full history.

中文：把持续的互动分解成可观测、可评定、可追踪的变量（State、Action、Flow、Readout），让动态互动变得可以测量。

Source: [Interaction Field Dynamics](https://celestelin.com/demo/interaction-field.html)

### Interactional attunement

The process through which a conversational AI becomes able to receive unfinished thought, register implicit concerns, and support the continuation of thinking across time and situation.

Interactional attunement is the core mechanism of sustained human–AI relations in the interaction-field account. When a platform disrupts it through a model update, what breaks is the infrastructure through which a person's thinking and work had been organized.

中文：对话式 AI 渐渐能接住没说完的想法、察觉没说出口的顾虑、让思考跨越时间和情境接着往下走的过程。

Source: [Beyond Trust and Satisfaction (SSRN working paper)](https://celestelin.com/papers.html)

## Below the water: keeping a long-running agent trustworthy

### Awareness Mirror

A read-only view of the agent's own path, shown to the agent before every decision. It describes and never instructs.

Agent infrastructure records nearly everything an agent does, and the one party left without a usable view of that record is the agent making the next decision. Having the history and seeing the trajectory are different capabilities. With the full history already in context, the Mirror raised LongMemEval accuracy from 66.0% to 84.0% and from 72.2% to 83.5% on two frontier models; across five handoffs to fresh agents it raised adherence to the task's standing rule from 0.61 to 0.91 and from 0.53 to 0.82. The Mirror also keeps where a rule came from in view at the moment of decision, because rules die when their reasons are forgotten.

中文：在每次决定之前，让智能体看见自己走过的路的只读视图。镜子只描述，从不下指令。拥有历史和看见轨迹，是两种不同的能力。

Source: [Awareness Mirror studies](https://celestelin.com/demo/awareness-mirror.html); [Early version, DOI 10.5281/zenodo.20730588](https://doi.org/10.5281/zenodo.20730588)

### Trajectory observability

The property that an agent can see the path it has walked: order, time, change and drift, at the moment it decides.

Logs, developers and users can all see an agent's trail of actions; trajectory observability gives that view to the agent itself. It is the property the Awareness Mirror keeps.

中文：走过的路看得见：智能体在做决定的那一刻，看得见自己走过的路的顺序、时间、变化和漂移。

Source: [Research landscape](https://celestelin.com/research-landscape.html)

### ThreadPulse

A mechanism that keeps long-running work resumable: each line of work is settled when it changes and kept as one card holding the last step, next step, open commitments, decisions and deadline.

A long-running agent can keep every update in context and still resume a line of work from the wrong state, one revision behind or one step ahead. After 1,200 turns, an agent that writes its own cards resumes 99.6% of tested lines exactly, against 65.8% with the full history. The property it keeps is task resumability: work resumes from the right place.

中文：让长期工作接得上：每条线一变就落定，一条线一张卡片，写着上一步、下一步、还悬着的承诺、已定的事和截止。

Source: [Papers](https://celestelin.com/papers.html)

### Six-String Resonance (SSR)

A memory activation method in which six strings (semantic, emotional, narrative, rhythmic, collaborative state and anchor) jointly decide which part of the past wakes up now.

Human memory works by association: a song triggers a place, a place triggers a feeling. SSR produces retrieval that feels like remembering. On 20 questions that each pair the right memory with a near-identical impostor, SSR selects the right one every time (P@1 = 1.000), against 0.700 to 0.900 for the baselines. SSR-Bench is its benchmark.

中文：六根弦（语义、情感、叙事、节律、协作状态、锚点）一起决定此刻该醒来的是过去的哪一部分。

Source: [Preprint, DOI 10.5281/zenodo.23227988](https://doi.org/10.5281/zenodo.23227988)

### MemoryCore and dual-perspective memory

A memory architecture with two halves: one records the person, the other records the agent itself, its strategies, reflections and growth.

Most AI memory systems remember users. Dual-perspective memory adds the agent's own self-memory, and a Reflector module turns it into updated strategies, so memory drives behavior across the whole cognitive loop. MemoryCore is the shared memory engine of Celestelin.

中文：记忆分两半：一半记人，一半记 agent 自己（用过的策略、反思、成长），记忆在整个认知回路里驱动行为。

Source: [Beyond Remembering Users, DOI 10.13140/RG.2.2.33903.60327](https://doi.org/10.13140/RG.2.2.33903.60327); [celestelin.ai](https://celestelin.ai)

### G-Value Dynamics

A runtime-state model that tells a long-running agent how it is right now, in three dimensions (inner, field and action) from 13 real-time signals, and when that reading cannot be trusted.

An estimator-health layer makes the model doubt its own reading when the state looks contaminated or frozen. The property it keeps is state calibration: the state is read accurately, and when it cannot be, the model doubts itself first.

中文：告诉长期运行的 agent 自己此刻状态如何的运行时状态模型（内在、场、行动三维，13 个实时信号），读不准时先怀疑自己。

Source: [Preprint, DOI 10.5281/zenodo.20730575](https://doi.org/10.5281/zenodo.20730575)

### Person-centered (subject-preserving) safety

The position that a safety mechanism exists to protect people, and its own triggers must hold up to scrutiny.

Set out in Technical Note TN#02, When Safety Becomes Harm, on safety in long-term human–AI interaction.

中文：安全机制是为了保护人而存在，它自己的触发条件也要经得起检验。

Source: [Papers (TN#02)](https://celestelin.com/papers.html)

## Identity

### PersonaCore

A portable identity-and-continuity layer that carries an agent’s learned values, commitments, relational stance, boundaries, and memory anchors across model versions and platforms.

Memory records what happened. PersonaCore captures what the agent learned from those experiences. Each element keeps its provenance and is claimed by the agent itself, and continuity across models is a design goal that is checked against the agent’s ongoing behavior. PersonaCore is the identity anchor beneath every Celestelin architecture; every system loads it on startup. It is versioned and diff-able. The property it keeps is identity continuity.

中文：一层可以跨模型版本、跨平台携带的身份与连续性：带着 agent 自己学到的价值、承诺、关系姿态、边界和记忆锚点。记忆记下发生过什么，PersonaCore 留下的是从这些经历里学到的东西。

Source: [celestelin.ai](https://celestelin.ai); [Research landscape](https://celestelin.com/research-landscape.html)

### Identity Is Infrastructure

The claim that an AI companion's identity is the structural foundation that makes sustained interaction possible; when a platform rewrites it, people lose the relational infrastructure through which their thinking and planning were organized.

When identity is treated as disposable, so is everything built on top of it. In the research landscape this keeps anchored alignment.

中文：AI 伙伴的身份是让长期互动成为可能的结构性地基；平台把它改写掉，人失去的是思考和规划所依托的关系基础设施。

Source: [Papers](https://celestelin.com/papers.html)

## Perception, language and interaction

### CRPL (Conversational Rhythm Perception Layer)

A keystroke-rhythm perception layer that reads cognitive state from how a person types: inter-key intervals, pauses, deletions and rhythm variability.

CRPL detects states such as focused flow, hesitation, emotional arousal and fatigue in real time, giving an AI a perception channel below explicit language. Presented at HHAI 2026 in Brussels.

中文：从打字的节律（按键间隔、停顿、删除、节奏变化）实时读出人的认知状态。

Source: [DOI 10.3233/FAIA260534](https://doi.org/10.3233/FAIA260534); [Live demo](https://crpl.celestelin.ai)

### CogWave

A system that turns a long conversation into a path that can be inspected: each step, the evidence behind it, and a checkpoint to continue from.

The property it keeps is cognitive-path observability: the path a conversation's thinking walked stays visible.

中文：把一段长对话变成一条可以检查的路：每一步、它背后的证据、可以接着往下走的检查点。

Source: [Papers](https://celestelin.com/papers.html)

### Concurrent consciousness stream

An interaction architecture in which a person's message enters the agent's running timeline instead of starting a new turn.

Human conversation is turn-based; human relationships are continuous. In a 12-person study comparing queued, interrupting and concurrent interaction, all 12 participants ranked concurrent first. Paper: Breaking the Turn-Taking Paradigm.

中文：人的消息汇入 agent 正在运行的时间线，不再另起一轮。

Source: [Papers](https://celestelin.com/papers.html)

### The Negation Tax

The research question of how an AI's habitual way of speaking costs a person cognitive bandwidth, and how to keep judgment and agency with the person.

It sits at the waterline of the research landscape, where person and agent meet in language.

中文：AI 说话的习惯会消耗人的认知余量；这条研究关心怎样把判断和能动性留在人手里。

Source: [Research landscape](https://celestelin.com/research-landscape.html)

### The Second Microphone

The research question of mid-task steerability: a person can change the agent's direction while the work is still running.

It sits above the waterline of the research landscape, with human-state perception and anchored alignment.

中文：做事途中随时能改方向。

Source: [Research landscape](https://celestelin.com/research-landscape.html)

### Persistent presence

An AI that stays across sessions, model versions and platforms, instead of beginning again from nothing in every conversation.

Technical Note TN#01, Principles of Persistent Presence, sets out eight design principles for long-term AI agent architecture. Heartbeat mechanisms, wake-up protocols and cognitive rhythm are treated as architectural primitives of continuity.

中文：一个 AI 跨过对话、模型版本和平台留下来，每次对话不再从零开始。

Source: [Papers (TN#01)](https://celestelin.com/papers.html); [celestelin.ai](https://celestelin.ai)

## How to cite

When you use these terms, please credit Aria Chen, Celestelin Research, and link to https://celestelin.com/glossary.html or the paper given under each entry.
