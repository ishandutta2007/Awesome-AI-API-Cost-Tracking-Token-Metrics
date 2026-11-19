# Awesome-AI-API-Cost-Tracking-Token-Metrics

## Top AI API Cost Tracking & Token Metrics Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on LLM Spend Attribution, Token Telemetry, AI Proxy Gateways, Coding-Agent Quota Monitors & FinOps for AI*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI API Cost Tracking & Token Metrics**. These tools meter prompt and completion token usage across multi-provider LLM APIs, enforce per-user/team budgets and rate limits, monitor local coding-agent subscription quotas (`Claude Code`, `Codex`, `Cursor`), and optimize AI FinOps via semantic caching and model routing.



**Examples** include Helicone, Langfuse, Portkey, PromptLayer, Martian, LiteLLM Proxy, Keywords AI, Cloudflare AI Gateway, Datadog LLM Observability, and phuryn/claude-usage (the category leaders). 



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted LLM cost/usage gateways, local CLI & statusline token meters, OpenTelemetry FinOps collectors, tokenizers/cost calculators, and multi-tenant quota managers — ideal for AI platform engineers, FinOps teams, and developers tracking token burn across local and cloud workflows.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing (Paid Tiers) | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Cloudflare AI Gateway](https://cloudflare.com)** | **~$68.7B Market Cap** ($2.17B FY25 Revenue) | $0 edge gateway fee on Free/BYOK; Workers Paid starts at **$5/month** (Unified Billing adds 5% credit processing fee) | **Free Forever plan**: Capped at 10 gateways, 100,000 total stored logs across account, 25 MB max cacheable request size, and 200 req/60s rate limit on unified billing. | Managed edge proxy sitting between applications and AI providers to deliver unified request analytics, token/cost estimation, response caching, and rate limiting. |
| **[Datadog LLM Observability](https://datadoghq.com)** | **~$48.5B Market Cap** ($3.43B FY25 Revenue) | Pro tier starts at **$160/month** (includes 100,000 LLM spans; additional spans billed in blocks) | **Free Forever plan**: 40,000 LLM spans/month with 15-day data retention; also offers a **14-day free trial** with full access to the observability suite. | Enterprise cloud monitoring solution tracking end-to-end LLM and agent traces, token consumption, operational spend, latency bottlenecks, and drift metrics. |
| **[LangSmith (LangChain)](https://langchain.com)** | **$3.0B Valuation** ($460M raised) | Plus plan starts at **$39/seat/month** (includes 10,000 base traces/month shared; overages at ~$2.50 per 1,000 traces) | **Developer Free Forever plan**: 1 seat, up to 5,000 traces/month, 14-day data retention, 10 dataset rows per dataset. | Enterprise AI engineering and observability platform by LangChain offering trace-level token accounting, run evaluations, prompt playground, and cost tracking. |
| **[Martian](https://withmartian.com)** | **~$1.3B Valuation** ($30M+ raised) | Usage routing fees starting at **$20 per 5,000 requests** or **$0.05/M tokens routed** on top of underlying model token costs; Enterprise custom contracts | **Case-by-case developer credit allocation**: Requires account signup and dashboard credit provisioning (no permanent self-serve free tier; promotional hackathon/research credits granted). | Model-routing and cost-optimization API platform that dynamically routes prompts to the most cost-effective LLM capable of meeting quality thresholds. |
| **[Arize AX](https://arize.com)** | **$915M Valuation** (Acquired by Dynatrace for $915M; $131M raised) | AX Pro starts at **$50/month** (50,000 spans/mo, 10 GB ingestion, 30-day retention; overage billing enabled) | **Free Forever plan**: 25,000 trace spans/month, 1 GB storage ingestion/month, 15-day data retention, 1 space, and 10 Signal issues/month. | Enterprise AI observability, evaluation, and tracing platform providing granular token accounting, cache-read/write token metrics, and cost anomaly alerts. |
| **[Portkey](https://portkey.ai)** | **~$140M Valuation** (Acquired by Palo Alto Networks; $18M+ raised) | Production plan starts at **$49/month** (includes 100,000 recorded logs/month with 30-day retention; overages at $9 per 100k requests) | **Developer Free Forever plan**: 10,000 recorded logs/month, 3-day log retention, 30-day metrics retention; requests beyond 10k continue routing without interruption (unlogged). | Enterprise AI gateway and observability suite featuring virtual API keys, granular budget caps, automatic fallback routing, semantic caching, and real-time cost dashboards. |
| **[Helicone](https://helicone.ai)** | **$25M Valuation** (Acquired by Mintlify; $5M Seed raised) | Pro plan starts at **$79/month** (+ usage-based overages; includes unlimited seats, 1-month retention); Team tier at $799/month | **Hobby Free Forever plan**: 10,000 requests/month, 1 GB storage, 7-day data retention, 1 seat, 1 organization, and rate limit of 10 logs/minute. | Proxy-based LLM observability and FinOps platform providing real-time token metering, per-user/property cost attribution, semantic caching, and custom rate-limit alerts. |
| **[PromptLayer](https://promptlayer.com)** | **~$4.8M Funding Raised** (ScOp & Stellation Capital Seed) | Pro plan starts at **$49/month** (unlimited workspaces and playgrounds, 150 MB dataset storage; overage at $0.003/transaction) | **Free Forever plan**: Up to 5 users, 2,500 requests/month, 1 workspace, 250 evaluation executions/month, 10 MB dataset storage, and 10 prompt templates. | Prompt management and LLM analytics platform providing request history logging, token-per-template cost breakdowns, latency tracking, and A/B test evaluations. |
| **[Keywords AI (Respan)](https://keywordsai.co)** | **Seed-funded** (Y Combinator W24) | Team plan starts at **$199/month** (higher proxy throughput ~8,400 req/min; optional HIPAA add-on at $500/month; overages at $8 per 100k logs) | **Free Forever plan**: $0/month with starter volume of up to 100,000 logs, 30-day log retention, up to 2 team seats, and 10 prompt template versions. | Unified LLM gateway and monitoring platform offering a single OpenAI-compatible endpoint with token analytics, latency metrics, user-level spend limits, and caching. |





## Open-Source GitHub Projects



- **[phuryn/claude-usage](https://github.com)**  

  Open-source macOS menu-bar utility and CLI monitor built for tracking real-time Claude Code and Claude subscription token consumption, 5-hour/weekly quota burn rates, and session costs.



- **[LiteLLM Proxy (`BerriAI/litellm`)](https://github.com)**  

  Leading open-source (`MIT`) AI gateway and Python SDK providing a unified OpenAI-compatible proxy across 100+ LLMs with virtual keys, team/user budget enforcement, and real-time spend tracking.



- **[Langfuse (`langfuse/langfuse`)](https://github.com)**  

  Self-hostable open-source LLM engineering platform featuring customizable model token pricing, hierarchical trace/session cost aggregation, and prompt-level spend dashboards.



- **[Helicone (`Helicone/helicone`)](https://github.com)**  

  Open-source (`Apache-2.0`) AI gateway and observability proxy enabling self-hosted request logging, token/cost metrics, caching, and rate limiting.



- **[Portkey AI Gateway (`Portkey-AI/gateway`)](https://github.com)**  

  Ultra-fast open-source (`MIT`) AI gateway written in TypeScript providing multi-provider routing, automatic retries, token/cost metadata headers, and lightweight self-hosting.



- **[TensorZero (`tensorzero/tensorzero`)](https://github.com)**  

  Open-source (`Apache-2.0`) industrial-grade LLM gateway, observability, and optimization engine written in Rust with ClickHouse-backed token, latency, and cost analytics.



- **[One-API / New-API (`MartialBE/one-api` / `Calcium-Ion/new-api`)](https://github.com)**  

  Popular open-source (`MIT`) multi-provider LLM key aggregation and billing gateway featuring token quota management, user groups, rate limiting, and detailed consumption logs.



- **[OpenLIT (`openlit/openlit`)](https://github.com)**  

  Open-source (`Apache-2.0`) OpenTelemetry-native AI observability and FinOps platform providing zero-code token/cost tracking, GPU metrics, and customizable pricing configurations.



- **[OpenLLMetry (`traceloop/openllmetry`)](https://github.com)**  

  Open-source (`Apache-2.0`) OpenTelemetry instrumentation extensions exporting standardized `gen_ai.usage.input_tokens` and `output_tokens` metrics to Prometheus, Grafana, or Datadog.



- **[ccusage (`ryoppippi/ccusage`)](https://github.com)**  

  Fast open-source (`MIT`) CLI analyzer for parsing local Claude Code JSONL logs to display daily, monthly, and session-level token usage, prompt cache hit rates, and equivalent API spend.



- **[Claude-Code-Usage-Monitor (`Maciek-roboblog/Claude-Code-Usage-Monitor`)](https://github.com)**  

  Real-time open-source (`MIT`) terminal dashboard tracking Claude Code token burn velocity, session reset countdowns, and predictive usage warnings.



- **[TokenCost (`AgentOps-AI/tokencost`)](https://github.com)**  

  Lightweight open-source (`MIT`) Python utility library for calculating exact USD prompt and completion costs across hundreds of commercial and hosted LLM models.



- **[tiktoken (`openai/tiktoken`)](https://github.com)**  

  Fast open-source (`MIT`) BPE tokenizer from OpenAI used across FinOps pipelines for accurate pre-flight token counting and context-window budget estimation.



- **[Bifrost (`maximhq/bifrost`)](https://github.com)**  

  High-throughput open-source (`Apache-2.0`) AI gateway built in Go featuring sub-millisecond overhead, virtual key budgets, fallback routing, and OpenTelemetry token metrics.



- **[RouteLLM (`lm-sys/RouteLLM`)](https://github.com)**  

  Open-source (`Apache-2.0`) framework from LMSYS for training and serving cost-aware LLM routers that dynamically dispatch simple queries to cheaper models while preserving quality.



- **[GPTCache (`zilliztech/GPTCache`)](https://github.com)**  

  Open-source (`MIT`) semantic caching library that intercepts repetitive LLM prompts and serves cached completions to dramatically reduce API token expenditure.



### Additional Strong Open-Source Options



- **[Lunary (`lunary-ai/lunary`)](https://github.com)** and **[Opik (`comet-ml/opik`)](https://github.com)** for self-hosted LLM observability suites with built-in per-user and per-trace cost dashboards.

- **[BricksLLM (`bricks-cloud/BricksLLM`)](https://github.com)** for an open-source Go-based cloud-native AI gateway with granular API key spend limits and rate policies.

- **[Grafana + Prometheus + OpenTelemetry Collector](https://github.com)** for building custom real-time FinOps token burn dashboards from standardized OpenTelemetry `gen_ai` metrics.

- **[Promptfoo (`promptfoo/promptfoo`)](https://github.com)** for benchmarking token efficiency and latency-vs-cost trade-offs across candidate prompts and models in CI/CD.

- **[vLLM](https://github.com)** and **[Ollama](https://github.com)** for self-hosting open-weight models with Prometheus token-throughput metrics to eliminate per-token cloud API fees.



**Frameworks for building custom systems**: Combine **LiteLLM Proxy** or **TensorZero** (for multi-provider budget enforcement & routing) with **Langfuse / OpenLIT** (for trace-level FinOps attribution), **phuryn/claude-usage / ccusage** (for local coding-agent quota tracking), and **TokenCost** for complete AI API cost visibility.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- LLM provider pricing, prompt-caching multipliers (`cache_read` / `cache_creation`), and reasoning-token billing rules change frequently — verify pricing tables regularly when relying on proxy cost estimates for chargebacks.
