# Tim Finnegan
 
Senior software engineer — production LLM systems, real-time simulation, and the infrastructure underneath both. Day job: leading AI and simulation work at a game studio. Nights: running a one-person platform team.
 
**Most of my original work lives on self-hosted infrastructure** — a Forgejo instance with CI and a private registry, deployed to a 4-node ARM64 K3s cluster behind zero-trust networking. I host my own forge for the same reason I sandbox my AI agents: I like knowing exactly what my tools can touch. Selected projects are mirrored here; ask me about the rest.
 
### Selected work
 
- **[forgejo-mcp](https://github.com/timFinn/forgejo-mcp)** (Go, original) — MCP server exposing 45 tools over the Forgejo API to LLM agents. stdio + HTTP transports, protocol handshake validated in CI. Started in TypeScript, deliberately rewritten in Go.
- **[OpenAlice](https://github.com/timFinn/OpenAlice)** (TypeScript/Node 22, active fork) — original feature work on an agentic trading platform: event-sourced architecture, multi-provider AI routing, approval-gated execution. See the fork notes in the README.
- **[weather-station](https://github.com/timFinn/weather-station)** (Python, original) — Raspberry Pi sensor pipeline (MQTT → InfluxDB → Grafana) that has run continuously in the field for months. I2C bus recovery, graduated error handling, Home Assistant discovery.
- **SpiderFoot v6** (Python, fork + major original work, self-hosted) — added the AI layer to an OSINT platform: LLM analysis agents on a Redis event bus, LiteLLM multi-provider gateway, Qdrant vector search, and LLM output sanitization to prevent data exfiltration. Happy to walk through it.
- **Homelab platform** (self-hosted) — GitOps K3s cluster (Cilium eBPF, ArgoCD, Longhorn), Tailscale policy-as-code, local LLM inference node (Ollama/MLX on Apple Silicon).
🌐 [timfinn.dev](https://timfinn.dev)
