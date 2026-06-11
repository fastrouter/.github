<div align="center">

# ⚡️FastRouter

**One API. Every Model. Production Ready.**

</div>

<div align="center">

[![Docs](https://img.shields.io/badge/Docs-0A0F1E?style=flat&logo=gitbook&logoColor=white)](https://docs.fastrouter.ai)
[![Free Audit](https://img.shields.io/badge/Free_Audit-0F172A?style=flat&logo=checkmarx&logoColor=white)](https://fastrouter.ai/audit)
[![Discord](https://img.shields.io/badge/Discord-0A0F1E?style=flat&logo=discord&logoColor=white)](https://discord.gg/QfTgEtMyyU)
[![X](https://img.shields.io/badge/X-0F172A?style=flat&logo=x&logoColor=white)](https://twitter.com/fastrouterai)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A0F1E?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/company/fastrouter-ai)

</div> 

<div align="left">

Unified LLM API gateway routing requests across 100+ models from OpenAI, Anthropic, Google, Meta, xAI, Cohere and more, through a single OpenAI-compatible endpoint.

**🔀 Intelligent Routing** : Auto-select models by cost, latency, or quality  
**🛡️ Governance** : Per-key budgets, RBAC, BYOK, spend alerts  
**📊 Observability** : Unified logs, tracing, latency quantiles across all providers  
**🧪 Evals & Quality** : Custom evals, prompt optimization, guardrails, caching  
**🔌 MCP Gateway** : Connect any MCP server, scoped per project  
**⚡ IDE Integrations** : Cursor, Cline, Claude Code,  Codex, Roo and lot many

</div>

---

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
<div align="center">
    
## [Sign up free: no credit card required!](https://fastrouter.ai/sign-up)

</div>
