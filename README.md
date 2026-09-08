<div align="center">

<img src="assets/banner.svg" alt="Basel Anaya — building the infrastructure layer for agents" width="100%"/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Basel_Anaya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/Basel-anaya)
[![Website](https://img.shields.io/badge/maximlabs.co-D97757?style=for-the-badge&logo=firefox&logoColor=white)](https://maximlabs.co)
[![Location](https://img.shields.io/badge/Amman,_Jordan-222222?style=for-the-badge)](#)

**AI Infrastructure Engineer · Solo Founder @ [Maximlabs](https://maximlabs.co)**

*Agents. Security. Markets. All local. All production.*

</div>

---

## [⬢ Cirax](https://github.com/baselanaya/Cirax) — now shipping

<div align="center">

<img src="assets/cirax.svg" alt="Cirax" width="92"/>

**An invisible AI copilot that floats over your screen — sees what you see,<br>hears your meetings, and stays hidden from screen shares.**

[![Release](https://img.shields.io/github/v/release/baselanaya/Cirax?style=flat-square&color=5B9BFF)](https://github.com/baselanaya/Cirax/releases)
[![CI](https://img.shields.io/github/actions/workflow/status/baselanaya/Cirax/ci.yml?branch=main&style=flat-square&label=CI)](https://github.com/baselanaya/Cirax/actions/workflows/ci.yml)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-3D6FD8?style=flat-square)]()
[![License](https://img.shields.io/badge/license-GPL--3.0--or--later-blue?style=flat-square)](https://github.com/baselanaya/Cirax/blob/main/LICENSE)

</div>

A free, self-hosted Cluely alternative. BYOK — OpenAI, Anthropic, Gemini, Azure, or any OpenAI-compatible endpoint — with everything sensitive staying on your machine:

- **Stealth where the OS allows it** — `WDA_EXCLUDEFROMCAPTURE` on Windows; honest per-platform reporting everywhere else (no fake promises)
- **Local Whisper STT** — microphone + meeting audio transcribed offline, keys encrypted via the OS keyring
- **Eye-contact camera companion** — a virtual webcam that corrects your gaze while you read answers, driven by a MobileGaze network at ~7 ms/frame on CPU
- **Real releases** — CI-built Linux x64/arm64 AppImages and a Windows installer on every version tag

`Electron` · `JavaScript` · `Whisper.cpp` · `ONNX Runtime` · `MediaPipe`

---

## Projects

| | |
|---|---|
| 🔐 **[Kernex](https://github.com/baselanaya/Kernex)** — zero-trust execution hypervisor for AI agents. A single static Rust binary that sandboxes any agent at the OS level with **Landlock LSM + seccomp BPF** — before the process boots. Audit mode generates least-privilege policies by observing one run; **< 2 ms overhead** vs ~500 ms for Docker. <br/>`Rust` `Landlock` `seccomp` `MCP` | 🗄️ **[Mercer](https://github.com/baselanaya/Mercer)** — text-to-SQL for messy production schemas. Six-stage agentic pipeline on a consumer GPU, no vector DB. **74% execution accuracy** on stratified benchmarks with Qwen2.5-Coder-7B, 100% on window functions. <br/>`Python` `llama.cpp` `Triton` `FastAPI` |
| 📈 **[Cynosure](https://github.com/baselanaya/Cynosure)** — fully local autonomous trading system for OKX perpetual swaps. A local Qwen3.5-4B synthesizer reads a ~500-token expert signal brief each 15-min cycle; deterministic Python owns all risk logic. Zero cloud LLM dependency. <br/>`Python` `TimesFM 2.5` `Ollama` `OKX` | 🗣️ **[Valerie](https://github.com/baselanaya/Valerie)** — visual speech recognition. A 500M-parameter VALLR-based lip-reading model that transcribes speech from video alone. <br/>`Python` `PyTorch` |
| 🛡️ **[Orion](https://github.com/baselanaya/Orion)** — self-hosted privacy VPN. Obfuscated WireGuard with a Tor-enforced Ghost mode. <br/>`Rust` `WireGuard` `Tor` | 🎬 **[Atlas](https://github.com/baselanaya/Atlas)** — multi-model AI soundtrack generation playground for cinematic and game composers. <br/>`Python` |
| 👻 **[RemnantUE5](https://github.com/baselanaya/RemnantUE5)** — first-person horror survival game in Unreal Engine 5.8, built as SAE Institute coursework. <br/>`C++` `UE5` | 🌐 **[Maximlabs](https://maximlabs.co)** — the umbrella for all of it: infrastructure for agents that run locally, execute safely, and act under clear rules. |

---

## Stack

<div align="center">

**Languages**

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)

**Inference & ML**

![llama.cpp](https://img.shields.io/badge/llama.cpp-D97757?style=for-the-badge)
![ONNX Runtime](https://img.shields.io/badge/ONNX_Runtime-005CED?style=for-the-badge)
![SGLang](https://img.shields.io/badge/SGLang-222222?style=for-the-badge)
![Triton](https://img.shields.io/badge/Triton_GPU_Kernels-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

**Systems & Infra**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Electron](https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## Stats

<div align="center">

<img width="495" src="https://streak-stats.demolab.com?user=baselanaya&theme=dark&hide_border=true&background=0d1117&ring=D97757&fire=D97757&currStreakLabel=D97757&sideLabels=c9d1d9&dates=c9d1d9&currStreakNum=ffffff&sideNums=ffffff" />

<br /><br />

<img width="495" src="https://github-readme-activity-graph.vercel.app/graph?username=baselanaya&bg_color=0d1117&color=c9d1d9&line=D97757&point=D97757&area=true&hide_border=true" />

</div>

---

<div align="center">

```
systems programming  ·  LLM inference  ·  agentic infrastructure  ·  kernel security
```

[maximlabs.co](https://maximlabs.co) · [LinkedIn](https://linkedin.com/in/Basel-anaya) · Amman, Jordan

</div>
