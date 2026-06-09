# FastRouter

**One API. Every Model. Production Ready.**

Unified LLM gateway routing requests across 100+ models: OpenAI, Anthropic, Google, Meta, xAI, Cohere and more: through a single OpenAI-compatible endpoint.

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

- **Routing**: Auto model selection, virtual aliases, fallbacks, provider strategies, free & flex pricing
- **Multimodal**: Chat, embeddings, image, audio, video, PDF, web search, realtime
- **Governance**: Per-key budgets, RBAC, BYOK, provisioning keys, spend alerts
- **Observability**: Unified dashboard, activity logs, tracing (W3C), latency quantiles
- **Evals & Quality**: Custom evals, prompt optimization (GEPA), guardrails, caching
- **MCP Gateway**: Connect any MCP server with OAuth 2.0, scoped per project, auto-execution
- **Batch Processing**: Up to 50K requests per job
- **IDE Integrations**: Cursor, Cline, Claude Code

## Links

[Docs](https://docs.fastrouter.ai) · [Dashboard](https://dashboard.fastrouter.ai) · [Free Audit](https://fastrouter.ai/audit) · [Sign up free](https://fastrouter.ai/sign-up)

[Discord](https://discord.gg/QfTgEtMyyU) · [X](https://twitter.com/fastrouterai) · [LinkedIn](https://linkedin.com/company/fastrouter-ai)
