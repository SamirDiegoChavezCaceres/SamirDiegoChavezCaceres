# Hi, I'm Samir 👋

Software/ML engineer working on an AdTech AI platform: LLM agents, retrieval,
and the production plumbing that keeps them honest (observability, data
pipelines, safe deploys). I like systems that fail loudly and tell you why.

- 🛠️ Python · LangGraph · FastAPI · PostgreSQL/pgvector · polars · Prometheus/Grafana · Power BI
- 🎓 Postgraduate studies in Data Science (UNSA)
- 🌎 Based in Peru

## Featured projects

Each repo is a small, self-contained, tested pattern - the kind of problem I
solve day to day, rewritten from scratch so it stands on its own.

| Project | What it shows |
|---------|---------------|
| [semantic-rag-pgvector](https://github.com/SamirDiegoChavezCaceres/semantic-rag-pgvector) | A RAG that says "I don't know": retrieval with a distance threshold, plus content-hash dedup over pgvector. |
| [langgraph-agent-hitl](https://github.com/SamirDiegoChavezCaceres/langgraph-agent-hitl) | A LangGraph agent with a hub router and a human-in-the-loop step that pauses for approval and resumes by token. |
| [cron-metrics-prometheus](https://github.com/SamirDiegoChavezCaceres/cron-metrics-prometheus) | Cron monitoring where the alert carries the real error, not just `exit=1`. Pushgateway + Prometheus + Grafana. |
| [sunedu-oferta-academica](https://github.com/SamirDiegoChavezCaceres/sunedu-oferta-academica) | A quota-aware client for Peru's public SUNEDU data and a polars star model with validations that fail loud. |

## A few things I care about

- **Honest failure.** "Found nothing" and "errored" are different answers; code
  should never paper over either with a confident guess.
- **Validate before you trust.** Especially joins across data sources - verify
  the values, not just the column names.
- **Make the alert useful.** The signal should carry enough context to act on
  without spelunking through logs.
