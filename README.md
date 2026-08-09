<h1 align="center">Daming Wu · 吴达明</h1>
<p align="center">
  <b>Founder-engineer building production AI products and GPU systems</b><br/>
  San Jose · Bilingual (EN/ZH) · Product surface to compute control plane
</p>
<p align="center">
  <a href="https://damingwu.com">damingwu.com</a> ·
  <a href="mailto:damingwu2026@gmail.com">damingwu2026@gmail.com</a>
</p>

<p align="center">
  <b>5.3×</b> fewer tokens · <b>122</b> tests · <b>1,321</b> videos unattended ·
  <b>60+</b> data sources · <b>5M+</b> daily reads
</p>

---

### Systems

| | System | What is under the hood | Evidence |
|---|---|---|---|
| 01 | **[Collie](https://collie.run)** | A coding agent that lives on your computer — and can actually run it. Terminal, desktop, browser and iOS. `Python` · `Swift` · `MCP` | Matched a comparable open agent on SWE-bench Verified using **5.3× fewer tokens** — ~110K against ~588K per instance, metered at the HTTP boundary by a proxy I wrote. |
| 02 | **[VocalCode](https://vocalcode.app)** | Local push-to-talk dictation for AI coding. Hold a configured key or mouse button, speak, and release; text is inserted into the active field in most desktop apps. `Rust` · `sherpa-onnx` · `WebView2` | **1.0.0 is live** for Windows and Apple silicon macOS, with signed/notarized installers, a 30-day full trial and a $4.99 one-time launch price. |
| 03 | **[Nestlyze](https://nestlyze.com)** | An AI buyer's agent for US homebuyers — a two-minute chat, then 24 matched homes with transparent valuations. `FastAPI` · `PostGIS` · `pgvector` · `React` | Six domain agents fuse **60+ public sources**; gradient-boosted valuation on a leakage-safe temporal split, served in ~10 ms. |
| 04 | **[Stay](https://thestay.app)** | Open-source, crisis-aware mental-health AI. 988 and Crisis Text Line escalation, conversations encrypted on the device. `Next.js` · `Claude` | Every safety rule is bound to a behavioral test in CI — **the policy runs**, it is not a document. |
| 05 | **dota-rl** | A Dota 2 bot trained offline from high-MMR human replays — behavioral cloning into offline RL, the AlphaStar-Unplugged pattern. `PyTorch` | **1M+ replay frames**. The live engine validates only; sanctioned Lua Bot API throughout — no injection, no memory reading. |
| 06 | **Video pipeline** | Whisper → LLM → a TTS cascade that degrades through three engines instead of failing a batch → FFmpeg → upload. `Python` · `CUDA` · `systemd` | **1,321 videos** published unattended across 23 accounts, VRAM-coordinated against concurrent GPU work. |
| 07 | **Cartek** | The auto marketplace I co-founded in 2018 and ran engineering for until 2025 — marketplace, ML, payments and infrastructure from zero. `Laravel` · `AWS` · `Stripe Connect` | Six engineers, **5M+ read requests a day at 99.9% uptime**, on a double-entry ledger with Stripe Connect as merchant of record. |
| 08 | **GPU systems lab** | A local resource broker and a cloud control plane for heterogeneous GPUs — priority, preemption, per-client VRAM quotas, gaming-mode yield, capability-aware placement and lease-based claims. `Python` · `NVML/CUDA` · `Cloudflare Workers` · `D1` | **122 tests** across scheduling, recovery and API behavior; register → enqueue → claim → complete validated end to end. |

### Open source

- **[colliehq/collie](https://github.com/colliehq/collie)** — the agent above. Local-first, cross-platform, one-click Windows installer.
- **[gpubroker](https://github.com/wudaming00/gpubroker)** — GPU resource broker with HTTP, Python and MCP interfaces.
- **[claude-voice](https://github.com/wudaming00/claude-voice)** — push-to-talk voice interface for Claude Code.
- **[stay](https://github.com/wudaming00/stay)** — private, public-good mental-health companion.
- **[nestlyze-mcp](https://github.com/wudaming00/nestlyze-mcp)** — real-estate search and due diligence from Claude Desktop or Claude Code.

### Also

- **Rapport** — local dual-channel session transcription for therapists; microphone and system loopback separated, offline, signed. `Rust`
- **Collie for iOS** — a SwiftUI client that tails and drives agent runs from a phone.
- **Doppel** — pronunciation training where the native reference is your own cloned voice saying your own sentence.

### How I build

- **Across the stack.** Interfaces, backend services, distributed control planes, ML pipelines and operations.
- **Evidence first.** Benchmarks are metered at system boundaries; safety policies run in CI; schedulers are tested through failure and recovery.
- **Hardware-aware.** A home lab spanning RTX 5090, 3080 and 1080 hardware is the test bed for resource management, observability and heterogeneous placement.
- **Founder ownership.** I have taken products from blank repository through customer-facing operation, payments and production support.

### Core tools

`Python` · `TypeScript` · `Rust` · `FastAPI` · `React` · `CUDA/NVML` · `PyTorch` · `SQLite/Postgres` · `Cloudflare Workers/D1` · `AWS` · `Prometheus` · `MCP`
