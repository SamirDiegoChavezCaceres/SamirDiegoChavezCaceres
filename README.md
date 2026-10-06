# Hi, I'm Samir 👋

Software/ML engineer working on AI: LLM agents, retrieval,
and the production plumbing that keeps them honest (observability, data
pipelines, safe deploys). I like systems that fail loudly and tell you why.

- 🛠️ Python · LangGraph · FastAPI · PostgreSQL/pgvector · polars · Prometheus/Grafana · Power BI
- 🎓 Postgraduate studies in Data Science (UNSA)
- 🌎 Based in Peru

## Featured projects

Each repo is a small, self-contained, tested pattern - the kind of problem I
solve day to day, rewritten from scratch so it stands on its own.

### LLM & agents

| Project | What it shows |
|---------|---------------|
| [semantic-rag-pgvector](https://github.com/SamirDiegoChavezCaceres/semantic-rag-pgvector) | A RAG that says "I don't know": retrieval with a distance threshold, plus content-hash dedup over pgvector. |
| [langgraph-agent-hitl](https://github.com/SamirDiegoChavezCaceres/langgraph-agent-hitl) | A LangGraph agent with a hub router and a human-in-the-loop step that pauses for approval and resumes by token. |
| [llm-observability-evals](https://github.com/SamirDiegoChavezCaceres/llm-observability-evals) | Tracing that no-ops without keys (Langfuse-ready) plus an LLM-as-judge evaluation harness. |

### Platform, reliability & data

| Project | What it shows |
|---------|---------------|
| [mutation-approval-plane](https://github.com/SamirDiegoChavezCaceres/mutation-approval-plane) | Propose/approve/execute for changes: idempotent, auditable, with separation of duties and a before-image concurrency check. |
| [capability-access-guard](https://github.com/SamirDiegoChavezCaceres/capability-access-guard) | Fail-closed, capability-based authorization with tenant isolation and machine-readable denial reasons. |
| [cron-metrics-prometheus](https://github.com/SamirDiegoChavezCaceres/cron-metrics-prometheus) | Cron monitoring where the alert carries the real error, not just `exit=1`. Pushgateway + Prometheus + Grafana. |
| [sunedu-oferta-academica](https://github.com/SamirDiegoChavezCaceres/sunedu-oferta-academica) | A quota-aware client for Peru's public SUNEDU data and a polars star model with validations that fail loud. |

### Research & applied ML

| Project | What it shows |
|---------|---------------|
| [lung-cancer-risk-ml](https://github.com/SamirDiegoChavezCaceres/lung-cancer-risk-ml) | Lung cancer risk from lifestyle questionnaires (SMOTE + XGBoost + LIME), ~96% F1. Code behind our IEEE Xplore paper. |
| [insurance-risk-api](https://github.com/SamirDiegoChavezCaceres/insurance-risk-api) | Health-risk classifier served over a Flask REST API, preprocessing baked into one sklearn pipeline. |
| [mushroom-classification](https://github.com/SamirDiegoChavezCaceres/mushroom-classification) | Edible-vs-poisonous classification with dtype-driven preprocessing; runs on synthetic data or the public UCI dataset. |
| [recipe-traffic-prediction](https://github.com/SamirDiegoChavezCaceres/recipe-traffic-prediction) | Predict high-traffic recipes; median imputation in-pipeline and precision chosen to match the business cost. |
| [biosignal-feature-extraction](https://github.com/SamirDiegoChavezCaceres/biosignal-feature-extraction) | Spectral band power (FFT) and wavelet energy (DWT) features from 1-D signals, with a classifier. |

## A few things I care about

- **Honest failure.** "Found nothing" and "errored" are different answers; code
  should never paper over either with a confident guess.
- **Validate before you trust.** Especially joins across data sources - verify
  the values, not just the column names.
- **Make the alert useful.** The signal should carry enough context to act on
  without spelunking through logs.
