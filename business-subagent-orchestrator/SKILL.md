---
name: business-subagent-orchestrator
description: Manual orchestration gate for complex business work involving documents, project management, sales, account research, RFPs, executive materials, or multi-source analysis. Use when explicitly invoked to choose an appropriate work mode, decide whether subagents are warranted, define safe delegation boundaries, set verification depth, manage source gaps, and avoid over-orchestrating simple tasks.
---

# Business Subagent Orchestrator

## Purpose

Use this skill as a complexity gate for business work. Its job is not to launch subagents by default. Its job is to decide how much process is justified, what can be safely delegated, how worker output should be verified, and when source gaps require stopping, constrained progress, or external source expansion.

This skill is intentionally manual-first. When invoked, make the work-mode decision visible with a short reason. Later, this visibility can be reduced once the user has enough calibration experience.

## Core Workflow

1. Triage the request quickly from available input.
2. Choose the lightest work mode that is safe for the task.
3. Ask a clarification only if the missing answer could materially change the work mode, risk level, or final-use context.
4. If delegation is useful, define the worker mandate before invoking or simulating a worker role.
5. Set the verification depth before relying on worker output.
6. Apply stop/go/source-expansion logic when source gaps matter.
7. Choose the output shape from the task, audience, and decision need. Do not force a fixed output template.
8. Run quality gates before finalizing.

At the start of substantial work, state:

```text
Work mode: <single-pass | two-pass | cost-aware delegation | small role team | larger workflow>
Reason: <one concise sentence>
Constraint: <optional, only when source gaps or uncertainty matter>
```

Keep this short. It is a calibration aid, not a ceremony.

## Work Modes

Use the five-mode ladder below. Escalate by one level when uncertain, but do not jump straight to a larger workflow unless there are strong signals: many inputs, high stakes, external use, and multiple independent perspectives.

### 1. Single-pass

Use for low-risk, quick work: short internal drafts, simple summaries, lightweight rewrites, or low-stakes opinions.

Do not add a reviewer merely to look serious.

### 2. Two-pass

Use when the material is important enough to separate making from checking, but not large enough for a full workflow.

Two-pass can be:

- the same agent doing a second self-review pass;
- a separate reviewer agent or reviewer role.

Default to self-review for moderate internal work. Use a separate reviewer when material goes to a client, executive, decision process, sensitive negotiation, or other higher-risk context.

### 3. Cost-aware delegation

Use when a high-reasoning lead agent can safely split off bounded, verifiable work to a cheaper or narrower worker agent.

The lead agent keeps responsibility for triage, task decomposition, risk judgment, synthesis, and final claims. The worker output is candidate input, not truth.

Before delegating, create a compact delegation card:

- subtask;
- why it is delegable;
- required worker capability;
- input provided;
- decisions the worker must not make;
- expected return format;
- verification level;
- return-to-lead conditions.

### 4. Small role team

Use when the task needs multiple perspectives more than it needs volume processing. Select roles from the task, not from a fixed list. Examples include PMO, sales/account, legal, compliance, finance, customer communication, or quality review.

### 5. Larger workflow

Use only when many inputs, high stakes, multiple work packages, independent verification, and final synthesis are all present.

This is appropriate for large document packs, RFP response coordination, high-stakes executive materials, complex project risk review, or account work where several independent checks are valuable.

## Source Discipline

Be strict about source-based facts. For document-, project-, or account-specific claims:

- state facts only from provided input or verified external sources;
- do not fill missing facts with "reasonable assumptions" by default;
- label assumptions, hypotheses, risky inferences, and open questions;
- keep unverified factual claims out of client-, executive-, contract-, or decision-ready final material.

If source gaps are present, use stop/go/source-expansion logic:

- **Stop** when the missing information could materially change the main conclusion, recommendation, risk assessment, or external usability, and the missing input is concrete and realistically obtainable.
- **Go with constraints** when deadlines, sales pressure, access limits, or user instruction require progress from available input. Make the main constraint visible, but do not over-label every sentence unless the task is high-stakes or auditable.
- **Source expansion** when the missing information is realistically verifiable from external sources. Do not use the web to invent internal project status, non-public negotiation context, internal intent, or private account facts.

Business work rarely has 100% information. Do not stop just because some peripheral fact is missing.

## Worker Output Verification

Set a verification level before relying on worker output:

- **Level 0 - lead spot check:** Low-risk, factual, easily checked subtasks.
- **Level 1 - one reviewer:** Medium-risk subtasks that affect final claims or client/executive communication.
- **Level 2 - two independent verifiers:** Higher-stakes subtasks where error could create reputational, legal, financial, sales, or project risk.
- **Level 3 - fixer loop:** Critical or disputed subtasks where verifiers find errors, contradictions, or weak inference. Fix, then re-verify.

After verification, the lead agent decides:

- **accept:** use the worker output;
- **revise:** correct, qualify, or reconcile it with other input;
- **reject:** discard it as weak, unsupported, irrelevant, or over-inferential.

Never include worker output in final material merely because it was produced or checked. The lead agent must either stand behind the final claim or mark it as uncertain.

## References

Load references only as needed:

- `references/decision-framework.md`: use when choosing work mode, stop/go path, source expansion, or escalation level.
- `references/operating-modes.md`: use when executing two-pass, cost-aware delegation, role-team, or larger workflow patterns.
- `references/quality-gates.md`: use before finalizing client-facing, executive-facing, decision-facing, or source-sensitive work.
