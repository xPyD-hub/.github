## xPyD-hub

Lightweight, rapidly deployable **Prefill-Decode (PD)** proxy for LLM serving — minimal setup, minimal maintenance.

### Projects

- **[xPyD-proxy](https://github.com/xPyD-hub/xPyD-proxy)**
  Rapidly deployable PD proxy server — scheduling, health monitoring, and dynamic instance management for prefill/decode.

### About

xPyD-proxy implements a two-phase serving pattern:
- **Prefill** — KV cache preparation on dedicated prefill nodes
- **Decode** — autoregressive token generation on decode nodes

The proxy handles round-robin / load-balanced scheduling, health checks, and hot-reload of instance configs. Designed for local dev and lightweight deployment.
