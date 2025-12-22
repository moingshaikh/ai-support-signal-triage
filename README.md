# AI Support Signal Triage Agent

This repository documents a **human-in-the-loop AI agent** designed to help support, product, and engineering teams triage incoming support signals in a structured, explainable way.

The focus of this project is **decision quality and reasoning**, not automation or production deployment.

## Quick navigation

- 📄 Full workflow guide (PDF): [`docs/workflow-guide-v2.3.pdf`](docs/workflow-guide-v2.3.pdf)
- 🧠 Agent prompt (copy/paste): [`agent/prompt.md`](agent/prompt.md)
- 📊 Sample input data: [`data/raw_signals_sample.csv`](data/raw_signals_sample.csv)
- ✅ Example output: [`data/triage_output_example.csv`](data/triage_output_example.csv)
- 🧪 Run log (baseline): [`runs/run-001.md`](runs/run-001.md)
- 🏗 Architecture notes: [`docs/architecture.md`](docs/architecture.md)
- ⚖️ Design decisions: [`docs/decisions.md`](docs/decisions.md)


## Problem

Support signals arrive from many channels such as email, chat, app feedback, and reviews.
They are often noisy, duplicated, and unstructured.

Teams spend significant time manually:

- Identifying what is urgent
- Grouping related issues
- Deciding who should act

This increases response time and raises the risk of missing critical incidents.

## Solution

This project defines an **AI Support Signal Triage Agent** that:

- Classifies support signals into operational categories
- Assigns conservative P0–P3 priorities
- Detects duplicates and clusters related issues
- Recommends a clear next action and owning team
- Explains why each decision was made
- Produces an executive-ready daily digest

The agent is intentionally designed as **decision support**, not autonomous automation.

## What this project is (and is not)

### This is:

- A reusable AI reasoning workflow
- Human-in-the-loop by design
- Explainable and conservative
- Reproducible at zero cost

### This is not:

- A production automation system
- A ticketing or auto-reply bot
- A framework showcase
- A commercial SaaS product

## How to use this repository

You can reproduce the agent behavior with **no paid tools**:

  1. Open a fresh ChatGPT conversation
  2. Copy the agent prompt from `agent/prompt.md`
  3. Paste the sample dataset from `data/raw_signals_sample.csv`
  4. Run the instruction described in the workflow guide
  5. Review the structured output and digest

Full step-by-step instructions are in `docs/workflow-guide-v2.3.pdf`.

Repository contents

`docs/`
Full workflow guide, architecture notes, and design decisions

`agent/`
The agent prompt treated as a specification, with a changelog

`data/`
Sample inputs and example outputs for reproducibility

`runs/`
Logged agent runs documenting changes, observations, and refinements

Author

Prepared by **[Moin Shaikh](https://www.linkedin.com/in/moingshaikh/)**, Business Analyst & Solutions Consultant
Date created: 2025-12-18
