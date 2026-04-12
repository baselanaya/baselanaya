<!-- Header -->
<div align="center">

```
╔══════════════════════════════════════════════════════════════╗
║           building the infrastructure layer for agents        ║
╚══════════════════════════════════════════════════════════════╝
```

# Basel Anaya

**AI Infrastructure Engineer · Solo Founder @ [Maximlabs](https://maximlabs.co)**

*Agents. Security. Markets. All local. All production.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Basel_Anaya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/Basel-anaya)
[![Website](https://img.shields.io/badge/maximlabs.co-D97757?style=for-the-badge&logo=firefox&logoColor=white)](https://maximlabs.co)
[![Location](https://img.shields.io/badge/Amman,_Jordan-🇯🇴-222222?style=for-the-badge)](#)

</div>

---

<div align="center">

```
 agents need boundaries.    queries need answers.    markets need clarity.
       ↓                           ↓                        ↓
    Kernex                       Mercer                  Cynosure
```

</div>

---

## 🔐 [Kernex](https://github.com/baselanaya/Kernex) — Zero-Trust Agent Hypervisor

[![Rust](https://img.shields.io/badge/Rust-1.75+-orange?style=flat-square&logo=rust&logoColor=white)](https://github.com/baselanaya/Kernex)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://github.com/baselanaya/Kernex/blob/main/LICENSE)
[![Release](https://img.shields.io/badge/release-v0.1.0-22c55e?style=flat-square)](https://github.com/baselanaya/Kernex/releases/tag/v0.1.0)
[![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-lightgrey?style=flat-square)](#)
[![Language](https://img.shields.io/badge/language-98%25_Rust-orange?style=flat-square&logo=rust)](#)

> *"Don't trust the model. Trust the kernel."*

OS-level execution sandbox for AI agents. A single statically-compiled Rust binary that intercepts syscalls in real time using **Linux Landlock LSM + seccomp BPF** — before the agent process even boots. No VMs. No daemons. No code changes required.

```bash
# Before
python my_agent.py

# After — fully sandboxed at the OS level
kernex run -- python my_agent.py
```

**Key capabilities:**
- 🛡️ **Audit mode** — auto-generates a least-privilege `kernex.yaml` policy by observing one run
- ⚡ **< 2ms boot overhead** vs ~500ms for Docker
- 🔒 **MCP co-sandboxing** — each MCP server gets its own independent policy
- 🧵 **JIT interception** — blocked actions prompt the user rather than crash the agent

`Rust` · `Landlock LSM` · `seccomp BPF` · `macOS Endpoint Security` · `Unix Domain Socket IPC`

---

## 🗄️ [Mercer](https://github.com/baselanaya/Mercer) — Text-to-SQL for Messy Schemas

[![Python](https://img.shields.io/badge/python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/baselanaya/Mercer)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://github.com/baselanaya/Mercer/blob/main/LICENSE)
[![Exec Accuracy](https://img.shields.io/badge/exec_accuracy-74%25-22c55e?style=flat-square)](#)
[![GPU](https://img.shields.io/badge/GPU-8GB_VRAM-76B900?style=flat-square&logo=nvidia&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-backend-009688?style=flat-square&logo=fastapi&logoColor=white)](#)

Plain English → accurate SQL, even on schemas with cryptic abbreviations (`cust_seg_cd`, `e_add`, `p_spec`), missing foreign keys, and inconsistent naming. Six-stage agentic pipeline running entirely on a consumer GPU — no vector database required.

```
Question → [Entity Retrieval] → [Schema Linking] → [Query Decomposition]
        → [Candidate Generation ×3] → [Execution + Scoring] → [Correction] → SQL
```

**Benchmark (Qwen2.5-Coder-7B, RTX 4070 Laptop):**

| Complexity | Exec Accuracy |
|---|---|
| Window functions | 100% (7/7) |
| Set operations | 100% (4/4) |
| Aggregation | 88% (7/8) |
| Basic SQL | 75% (6/8) |
| **Overall (50 stratified)** | **74%** |

`Python` · `llama.cpp` · `Qwen2.5-Coder-7B` · `Triton` · `FastAPI` · `React` · `Redis` · `SQLAlchemy`

---

## 📈 [Cynosure](https://github.com/baselanaya/Cynosure) — Fully Local AI Trading System

[![Python](https://img.shields.io/badge/python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/baselanaya/Cynosure)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://github.com/baselanaya/Cynosure)
[![Status](https://img.shields.io/badge/status-active_development-3b82f6?style=flat-square)](#)
[![Exchange](https://img.shields.io/badge/exchange-OKX_perpetual_swaps-000000?style=flat-square)](#)
[![Cycle](https://img.shields.io/badge/cycle-15_min_24%2F7-D97757?style=flat-square)](#)

> *"Follow the star. Trade with clarity."*

Autonomous perpetual swap trading system for OKX — crypto majors, gold/silver, US equity index perps. Zero cloud LLM dependency. A local **Qwen3.5-4B** synthesizer reads a pre-computed expert signal brief (~500 tokens) and outputs a single structured JSON decision; all risk logic runs in deterministic Python.

```
15-min cycle:
  Expert Pipeline → MarketBrief (~500 tok) → LLM Synthesis (5-8s)
  → Signal Persistence Gates → Risk Engine (Kelly sizing) → OKX Execution
```

**Signal sources per cycle:** EMA/RSI/MACD/OFI across 3 timeframes · TimesFM 2.5 zero-shot forecast · L2 orderbook depth · Fear & Greed · funding rates · open interest · liquidation clusters

`Python` · `Qwen3.5-4B` · `Ollama` · `TimesFM 2.5` · `OKX MCP` · `SQLite` · `APScheduler`

---

## 👁️ [Valerie](https://github.com/baselanaya/Valerie) — Visual Speech Recognition

[![Python](https://img.shields.io/badge/python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/baselanaya/Valerie)
[![Params](https://img.shields.io/badge/parameters-500M-8B5CF6?style=flat-square)](#)
[![Architecture](https://img.shields.io/badge/architecture-VALLR-8B5CF6?style=flat-square)](#)

500M parameter lip-reading model. VALLR-based architecture that transcribes speech from video without audio.

`Python` · `PyTorch` · `VALLR`

---

## 🛠️ Stack

<div align="center">

**Languages**

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**Inference & ML**

![llama.cpp](https://img.shields.io/badge/llama.cpp-D97757?style=for-the-badge)
![SGLang](https://img.shields.io/badge/SGLang-222222?style=for-the-badge)
![Triton](https://img.shields.io/badge/Triton_GPU_Kernels-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

**Systems & Infra**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## 📊 Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=baselanaya&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=D97757&icon_color=D97757&text_color=c9d1d9&rank_icon=github" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=baselanaya&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=D97757&text_color=c9d1d9&langs_count=6" />

</div>

---

<div align="center">

```
systems programming · LLM inference · agentic infrastructure · kernel security
```

[maximlabs.co](https://maximlabs.co) · [LinkedIn](https://linkedin.com/in/Basel-anaya)

*Building in Amman, Jordan 🇯🇴*

</div>
