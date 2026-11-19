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



- **[Helicone](https://helicone.ai)**  

  Proxy-based LLM observability and FinOps platform providing real-time token metering, per-user/property cost attribution, semantic caching, and custom rate-limit alerts.



- **[Langfuse Cloud](https://langfuse.com)**  

  Managed cloud deployment of the open-source LLM engineering platform offering automated model pricing tables, trace-level token/cost rollups, and session spend analytics.



- **[Portkey](https://portkey.ai)**  

  Enterprise AI gateway and observability suite featuring virtual API keys, granular budget caps, automatic fallback routing, semantic caching, and real-time cost dashboards.



- **[Keywords AI](https://keywordsai.co)**  

  Unified LLM gateway and monitoring platform offering a single OpenAI-compatible endpoint with token analytics, latency metrics, user-level spend limits, and caching.



- **[Cloudflare AI Gateway](https://cloudflare.com)**  

  Managed edge proxy sitting between applications and AI providers to deliver unified request analytics, token/cost estimation, response caching, and rate limiting.



- **[Datadog LLM Observability](https://datadoghq.com)**  

  Enterprise cloud monitoring solution tracking end-to-end LLM and agent traces, token consumption, operational spend, latency bottlenecks, and drift metrics.



- **[PromptLayer](https://promptlayer.com)**  

  Prompt management and LLM analytics platform providing request history logging, token-per-template cost breakdowns, latency tracking, and A/B test evaluations.



- **[Martian](https://withmartian.com)**  

  Model-routing and cost-optimization API platform that dynamically routes prompts to the most cost-effective LLM capable of meeting quality thresholds.



- **[Arize AX / LangSmith](https://langchain.com)**  

  Enterprise AI engineering and observability platforms offering detailed token accounting, cache-read/write token breakdowns, and project-level cost alerts.





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
