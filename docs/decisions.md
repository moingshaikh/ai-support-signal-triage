# Design Decisions

This document captures key design decisions made while building the AI Support Signal Triage Agent.
It is intended to explain *why* certain tradeoffs were chosen.

- Human-in-the-loop by default
- Conservative escalation to avoid alert fatigue
- Explainability required for every decision
- Zero-cost validation before automation

---

See also:
- Architecture overview: [`architecture.md`](architecture.md)
- Run logs: [`../runs/run-001.md`](../runs/run-001.md)
