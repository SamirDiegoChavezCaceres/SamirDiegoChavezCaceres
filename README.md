# Hi, I'm Samir 👋

Software/ML engineer working on AI: LLM agents, retrieval, and the production
plumbing around them (observability, data pipelines, safe deploys). I like
systems that fail loudly and tell you why.

- 🛠️ Python · LangGraph · FastAPI · PostgreSQL/pgvector · polars · Prometheus/Grafana · Power BI
- 🎓 Postgraduate studies in Data Science (UNSA)
- 🌎 Based in Peru

## Featured projects

Each repo is small, self-contained, and stands on its own, with a demo GIF,
tests, and green CI.

### LLM & agents

| Project | What it shows |
|---------|---------------|
| [semantic-rag-pgvector](https://github.com/SamirDiegoChavezCaceres/semantic-rag-pgvector) | A RAG that says "I don't know": retrieval with a distance threshold, plus content-hash dedup over pgvector. |
| [graph-rag](https://github.com/SamirDiegoChavezCaceres/graph-rag) | Graph RAG: build a knowledge graph from text and answer multi-hop questions (A to B to C) that flat vector RAG misses. |
| [hybrid-search-rrf](https://github.com/SamirDiegoChavezCaceres/hybrid-search-rrf) | Hybrid search: keyword + vector retrieval fused with Reciprocal Rank Fusion, the retrieval setup behind good RAG. |
| [langgraph-agent-hitl](https://github.com/SamirDiegoChavezCaceres/langgraph-agent-hitl) | A LangGraph agent with a hub router and a human-in-the-loop step that pauses for approval and resumes by token. |
| [llm-observability-evals](https://github.com/SamirDiegoChavezCaceres/llm-observability-evals) | Tracing that no-ops without keys (Langfuse-ready) plus an LLM-as-judge evaluation harness. |

### Platform, reliability & data

| Project | What it shows |
|---------|---------------|
| [mutation-approval-plane](https://github.com/SamirDiegoChavezCaceres/mutation-approval-plane) | Propose/approve/execute for changes: idempotent, auditable, with separation of duties and a before-image concurrency check. |
| [transactional-outbox](https://github.com/SamirDiegoChavezCaceres/transactional-outbox) | The transactional outbox pattern: write a change and its event atomically, relay at-least-once, consume idempotently. |
| [capability-access-guard](https://github.com/SamirDiegoChavezCaceres/capability-access-guard) | Fail-closed, capability-based authorization with tenant isolation and machine-readable denial reasons. |
| [cron-metrics-prometheus](https://github.com/SamirDiegoChavezCaceres/cron-metrics-prometheus) | Cron monitoring where the alert carries the real error, not just `exit=1`. Pushgateway + Prometheus + Grafana. |
| [sunedu-oferta-academica](https://github.com/SamirDiegoChavezCaceres/sunedu-oferta-academica) | A quota-aware client for Peru's public SUNEDU data and a polars star model with validations that fail loud. |
| [email-intake](https://github.com/SamirDiegoChavezCaceres/email-intake) | Turn inbound email into a safe structured record: parse, scan attachments, redact PII, extract fields. |

### Research & applied ML

| Project | What it shows |
|---------|---------------|
| [lung-cancer-risk-ml](https://github.com/SamirDiegoChavezCaceres/lung-cancer-risk-ml) | Lung cancer risk from lifestyle questionnaires (SMOTE + XGBoost + LIME), ~96% F1. Code behind our [IEEE Xplore paper](https://doi.org/10.1109/ICA-ACCA62622.2024.10766818). |
| [insurance-risk-api](https://github.com/SamirDiegoChavezCaceres/insurance-risk-api) | Health-risk classifier served over a Flask REST API, preprocessing baked into one sklearn pipeline. |
| [mushroom-classification](https://github.com/SamirDiegoChavezCaceres/mushroom-classification) | Edible-vs-poisonous classification with dtype-driven preprocessing; runs on synthetic data or the public UCI dataset. |
| [recipe-traffic-prediction](https://github.com/SamirDiegoChavezCaceres/recipe-traffic-prediction) | Predict high-traffic recipes; median imputation in-pipeline and precision chosen to match the business cost. |
| [biosignal-feature-extraction](https://github.com/SamirDiegoChavezCaceres/biosignal-feature-extraction) | Spectral band power (FFT) and wavelet energy (DWT) features from 1-D signals, with a classifier. |

## A few things I care about

- **"Found nothing" and "errored" are different answers.** Code should not paper
  over either one with a confident guess.
- **Validate before you trust.** Especially joins across data sources: check the
  values, not just the column names.
- **Make the alert useful.** The signal should carry enough context to act on
  without spelunking through logs.
