## Ibram Ghali

**Senior AI Engineer, Melbourne.** I design, ship and govern production AI: LLM pipelines, AI agents, RAG assistants and the evaluation that makes them safe to rely on.

[LinkedIn](https://www.linkedin.com/in/ibramghali) · Portfolio (coming soon)

### What I have built in production

- **Internal AI platform** for a multi-country education group: one portal for six departments, a tool-using assistant over a document knowledge base, PII redaction, usage and cost tracking per tool
- **LLM compliance review of sales calls**: replaced three 60-step low-code workflows with one config-driven pipeline. A cheap model extracts, a stronger model judges, rules live as data, and reviewer feedback improves the rules. Thousands of calls a month
- **AI tax-statement SaaS** for accounting firms: every figure from exact decimal code and about 20 cross-source validation rules, with one read-only AI call for the reviewer's commentary. Multi-tenant on Azure, about 1,100 tests
- **Voice AI receptionist**: tool-calling voice agent for availability, booking and callbacks, with CRM write-back and knowledge synced from documents
- **Scheduled content agents** with human approval gates, token budgets and an AI quality check that flags but never publishes on its own

The repos below are public rebuilds of these patterns on synthetic data. Happy to walk through the production versions, get in touch.

### Selected work

| Repo | What it shows | Result |
| --- | --- | --- |
| [llm-compliance-judge](https://github.com/IbramGhali/llm-compliance-judge) | Two-stage LLM judge, verbatim-evidence checks, human review queue, CI regression gate | Golden-set macro F1 0.89, kappa 0.90; ~$0.03 per call |
<!-- Add rows as each new repo goes public: tax-statement-engine, rag-slack-assistant, voice-ai-receptionist, llm-gateway -->

### Stack

- **AI:** Claude, GPT, Gemini, MCP, structured outputs, RAG with pgvector and hybrid search, LLM evaluation
- **Engineering:** Python, TypeScript, FastAPI, Next.js, Celery, Postgres, Redis, Docker, GitHub Actions
- **Cloud and data:** Azure, GCP, Vercel, Supabase, BigQuery, dbt

### How I work

Code for everything deterministic, LLMs only where judgement is needed. Prompts, rules and models managed as data. Every AI output evaluated, monitored and reviewable by a human.
