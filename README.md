# FastRouter

**One API. Every Model. Production Ready.**

FastRouter is a unified LLM API gateway — a control plane for routing, managing, and observing requests across 100+ models from OpenAI, Anthropic, Google, Meta, xAI, Cohere, and more through a single OpenAI-compatible endpoint.

## What's here

This org contains the public documentation, integration guides, and API reference for FastRouter.

- **Docs** → [docs.fastrouter.ai](https://docs.fastrouter.ai)
- **Dashboard** → [dashboard.fastrouter.ai](https://dashboard.fastrouter.ai)
- **Free Audit** → [fastrouter.ai/audit](https://fastrouter.ai/audit)

## Quick start

```python
from openai import OpenAI

client = OpenAI(
    api_key="YOUR_FASTROUTER_KEY",
    base_url="https://go.fastrouter.ai/api/v1"
)

response = client.chat.completions.create(
    model="fastrouter/auto",
    messages=[{"role": "user", "content": "Hello"}]
)
```

## Features

### Routing
- **Automatic Model Selection** — `fastrouter/auto` picks the best model by cost, latency, or quality
- **Virtual Model Aliases** — group models under one alias; strategies: Random Shuffle, Lowest Latency, Highest Throughput, Lowest Usage, Lowest Price, Priority, Category-Based
- **Fallback Models** — sequential failover across providers on error or rate limit
- **Provider Routing Strategies** — `order`, `allow_fallbacks`, `only`, `ignore`, `sort` (`:price`, `:throughput`, `:latency` suffixes)
- **Free Models** — append `:free` to any supported model ID
- **Flex Pricing** — append `:flex` for up to 50% lower cost on latency-tolerant workloads

### Multimodal
- Chat completions, embeddings, image generation & editing, audio (TTS + STT), video generation, PDF processing, web search, realtime API, moderations

### API Compatibility
- OpenAI Chat Completions (primary)
- OpenAI Responses API
- Anthropic Messages Format
- Gemini Native Format

### Governance & Cost Control
- Per-project budgets and per-key rate limits
- RBAC — organization, members, roles
- BYOK (Bring Your Own Keys)
- Provisioning keys
- Dynamic tags per request for cost allocation
- Spend alerts
- Credits management

### Observability
- Unified dashboard — requests, cost, tokens, latency, errors across all providers
- Activity log with full request/response detail and content logging controls
- Latency distribution (P50, P90, P99), TTFT tracking
- W3C `traceparent` tracing — group LLM calls into spans, visualize in Traces view

### Evaluation & Quality
- Custom evaluations with LLM-as-a-judge
- Video evaluations
- Prompt Optimizations (GEPA-powered) — auto-improve system prompts with iterative scoring
- Prompt caching and response caching
- Guardrails
- Structured outputs, function calling, reasoning tokens

### MCP Gateway
- Register any MCP-compatible server (GitHub, Linear, Gmail, or custom APIs)
- Centralized credential management — OAuth 2.0 and static header auth
- Selective tool exposure per project
- Auto-execution mode with configurable `max_tool_rounds`

### Integrations
- IDE: Cursor, Cline, Claude Code
- OpenClaw
- Hermes Agent

### Processing
- Batch processing (up to 50K requests)

## Get started free

No credit card required. [Sign up →](https://fastrouter.ai/sign-up)

## Connect

- [Twitter / X](https://twitter.com/fastrouterai)
- [LinkedIn](https://linkedin.com/company/fastrouter-ai)
- [Discord](https://discord.gg/QfTgEtMyyU)
