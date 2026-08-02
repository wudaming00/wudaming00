<h1 align="center">Daming Wu · 吴达明</h1>
<p align="center">
  <b>Founder-engineer building production AI products and GPU systems</b><br/>
  San Jose · Bilingual (EN/ZH) · Product surface to compute control plane
</p>
<p align="center">
  <a href="https://damingwu.com">damingwu.com</a> ·
  <a href="mailto:damingwu2026@gmail.com">damingwu2026@gmail.com</a>
</p>

---

### Systems I'm building

| System | What is under the hood | Evidence |
|---|---|---|
| **[Collie](https://collie.run)** | Local-first coding agent across terminal, desktop, browser and iOS. Python · Swift · MCP. | Matched a comparable open agent on SWE-bench Verified with **5.3× fewer tokens**, metered at the HTTP boundary. |
| **GPU resource broker** | Priority, preemption, per-client VRAM quotas, gaming-mode yield, Prometheus telemetry and crash-recoverable state. Python · NVML/CUDA · SQLite. | **122 tests** across scheduling, recovery and API behavior. |
| **Heterogeneous GPU control plane** | Authenticated worker heartbeats, capability/VRAM-aware placement, priority queues, lease-based claims and lifecycle events. Cloudflare Workers · D1. | Register → enqueue → claim → complete path validated end to end. |
| **[VocalCode](https://vocalcode.app)** | Local speech-to-text at the OS caret with signed native binaries and an end-to-end checkout/license path. Rust · Whisper · Stripe. | Shipping at 0.4.9. |
| **[Nestlyze](https://nestlyze.com)** | Six domain agents fuse 60+ public sources behind transparent home valuation and risk signals. FastAPI · PostGIS · pgvector · React. | Live product; leakage-safe temporal model evaluation. |

### Other shipped systems

- **[Stay](https://thestay.app)** — crisis-aware, private mental-health AI whose safety rules are executable CI tests. `Next.js` · `Claude`
- **Video localization pipeline** — Whisper → LLM → resilient TTS cascade → FFmpeg → upload; 1,321 videos across 23 accounts. `Python` · `CUDA` · `systemd`
- **Cartek** — auto marketplace I co-founded and led technically for seven years; six engineers, 5M+ daily reads at 99.9% uptime. `Laravel` · `AWS` · `Stripe Connect`

### Open source

- **[gpubroker](https://github.com/wudaming00/gpubroker)** — GPU resource broker with HTTP, Python and MCP interfaces.
- **[claude-voice](https://github.com/wudaming00/claude-voice)** — push-to-talk voice interface for Claude Code.
- **[stay](https://github.com/wudaming00/stay)** — private, public-good mental-health companion.
- **[nestlyze-mcp](https://github.com/wudaming00/nestlyze-mcp)** — real-estate search and due diligence from Claude Desktop or Claude Code.

### How I build

- **Across the stack.** Interfaces, backend services, distributed control planes, ML pipelines and operations.
- **Evidence first.** Benchmarks are metered at system boundaries; safety policies run in CI; schedulers are tested through failure and recovery.
- **Hardware-aware.** A home lab spanning RTX 5090, 3080 and 1080 hardware is the test bed for resource management, observability and heterogeneous placement.
- **Founder ownership.** I have taken products from blank repository through customer-facing operation, payments and production support.

### Core tools

`Python` · `TypeScript` · `Rust` · `FastAPI` · `React` · `CUDA/NVML` · `PyTorch` · `SQLite/Postgres` · `Cloudflare Workers/D1` · `AWS` · `Prometheus` · `MCP`
