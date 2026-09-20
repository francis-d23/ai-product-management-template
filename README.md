# Juno PM — Rocket Ships Triage AI CoPilot

> An AI Associate PM that turns Slack/Notion/Jira chaos into a prioritised top-3 risk list every morning.

_Francis Delusong · AI PM Cohort · September 2026_

Repo: https://github.com/francis-d23/ai-product-management-template

This repo is my final project for the AI Product Management Certification — **Juno PM**. Each module’s artefact lives in its own folder; this README is the dashboard and the pitch.

---

## Module artefacts

### M1 · Prompting
- **System prompt** — [`https://github.com/francis-d23/ai-product-management-template/tree/main/01-prompting`](https://github.com/francis-d23/ai-product-management-template/tree/main/01-prompting)
- **Prototype** — https://your-build-tool/share/your-juno-prototype

### M2 · Strategy
- **Decision matrix** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/02-strategy/decision-matrix.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/02-strategy/decision-matrix.md)
- **AI Strategy one-pager** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/02-strategy/strategy-one-pager.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/02-strategy/strategy-one-pager.md)

### M3 · RAG / AI PRD
- **AI PRD** — [`https://github.com/francis-d23/ai-product-management-template/tree/main/03-rag-prd`](https://github.com/francis-d23/ai-product-management-template/tree/main/03-rag-prd)

### M4 · AI-Native UX
- **AI user flow** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/04-ai-ux/user-flow.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/04-ai-ux/user-flow.md)
- **Trust-gap mitigations** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/04-ai-ux/trust-gaps.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/04-ai-ux/trust-gaps.md)

### M5 · Agentic Workflows
- **Agent Workflow Spec (AWSpec)** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/05-agentic-workflows/awspec.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/05-agentic-workflows/awspec.md)
- **Agent Control Panel** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/05-agentic-workflows/agent-control-panel.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/05-agentic-workflows/agent-control-panel.md)

### M6 · Evals &amp; Guardrails
- **Eval stack** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/06-evals/eval-stack.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/06-evals/eval-stack.md)
- **Human evaluation rubric** — [`https://github.com/francis-d23/ai-product-management-template/blob/main/06-evals/human-rubric.md`](https://github.com/francis-d23/ai-product-management-template/blob/main/06-evals/human-rubric.md)

---

## PM Execution Plan

### Where Juno is today
- M1–M6 specced and committed.
- The prototype validates the M1 flow with the team.
- Automated evals: 250-item golden set drafted, judge prompt validated against 30 items; not yet wired to CI.
- Human rubric drafted; 2 grader candidates lined up; no calibration round yet.
- PM reviews any P0 with confidence < 75% before posting. Daily 9:00am: PM has a 10-min review window before the agent auto-posts to

### What ships next (next 2 sprints)
- Sprint 1: wire the eval harness to CI; staff and calibrate 2 graders; ship the triage tool.
- Sprint 2: open closed beta with 3 PMs (1 RocketShip, 2 customers); weekly rubric review; instrument abandon-rate.

### What I watch (dashboards)
- Daily: thumbs-down rate, regen rate, hand-off rate.
- Weekly: human-rubric mean per dimension; refusal hit-rate; cost per run.
- Per release: golden-set accuracy; format/citation/refusal pass rate.

### Red lines (what blocks shipping)
- Any critical-safety fail (any "0" on safety dimension in human eval).
- <90% golden-set accuracy on automated layer.
- Customer-name fabrication in last 30 days.
- Cost >$0.18 per run.
- P95 latency >15s on triage flow.

### Governance
- Compliance: PII scrubber pre-LLM; GDPR DSR handler in /docs/dsr-runbook.md.
- Safety: prompt-injection eval row in golden set; refusal on legal/contract content.
- Reliability: 99.5% SLO; cached top-3 fallback if model is down.
- Reputation: 2-hour incident-response playbook in /docs; canary deploys for every model swap.

---

## Build Insights

- **Friction point.** Time and effort to developing and designing a AI PRD Harness.  Note;  ProductSchool Modules were changing throughout the course making it difficult to reconcile project work.
- **Key learning.** Always build and incorporate strategic guadrails - Governance must be at the core to mitigage liability and risk
- **Aha moment.** System prompt sets the specific outputs that I would like to see OR it is already part of the Model to naturally do that

---

_Certification submission — AI Product Management Certification._
