# ai-eval-harness

**LLM evaluation & guardrail harness**  
Author: Saket Chamarti

Purpose: small, auditable evaluation system for LLM outputs in financial research contexts — metrics, hallucination checks, prompt-injection tests, and simple guardrails.

---

## Project overview

This project provides:
- `eval/` — scripts to compute evaluation metrics (pass@k, accuracy, hallucination rate, latency/cost metrics).
- `guardrails/` — prompt-injection detection & policy enforcement modules.
- `api/` — small FastAPI app to host evaluation endpoints.
- `notebooks/` — demo notebooks illustrating evaluation & reporting.
- `docker/` — Dockerfile for containerization.

---

## Quick start (local dev)

1. Clone & install:
```bash
git clone git@github.com:<your-org>/ai-eval-harness.git
cd ai-eval-harness
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
