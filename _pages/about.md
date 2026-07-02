---
layout: about
title: about
permalink: /
subtitle: An LLM researcher who gazes at the starlit skies of Artificial General Intelligence

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <p>M.S. in Intelligent Information Systems</p>
    <p>Carnegie Mellon University</p>
    <p>Language Technologies Institute</p>

selected_papers: true
social: true

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
---

Hi there! I'm **Gaokai Zhang**, an M.S. student in [Intelligent Information Systems](https://miis.cs.cmu.edu/) at CMU LTI since Fall 2025. I hold dual B.S. degrees from [ZJUI](https://zjui.intl.zju.edu.cn/en/) (CompE @ UIUC, ECE @ ZJU).

Currently, I'm interning at **NVIDIA** on agentic-workflow tooling and tokenomics, and contributing to [**sglang-omni**](https://github.com/sgl-project/sglang-omni). I also work with [Yiqing Xie](https://yiqingxyq.github.io/) and [Prof. Daniel Fried](https://dpfried.github.io/) on code-generation data synthesis and agent training.

**Open to LLM-related MLE/RS opportunities as I'm graduating in December 2026!**

---

### Experience

**NVIDIA** (May 2026 - Present)
*Software Engineer Intern, AI Tools Team*

- Built hook- and skill-based guardrails spanning 5 check categories (secrets, security, code quality, dependency, merge-conflict) that scan AI coding-agent actions in real time
- Contributed to token-saving agent-workflow skills benchmarked (N=50) against baseline harnesses on SWE-Bench Lite, Terminal-Bench, and CodeScaleBench, showing accuracy parity or improvement alongside uniform cost reduction — e.g., -38% cost with no accuracy loss on CodeScaleBench, and +7% accuracy at -12% cost on SWE-Bench Lite
- Built session-level hooks that capture agent-event telemetry — per-session token/cost usage, model-routing decisions, and subagent fan-out (turns, tokens) — feeding cost-governance dashboards

**sglang-omni** (Apr 2026 - Present)
*Open Source Contributor, [SGLang Project](https://github.com/sgl-project/sglang-omni)*

- Added native serving support for 5 TTS model families (Qwen3-TTS, Voxtral-TTS, OpenMOSS MOSS-TTS Delay + Local-Transformer, Zyphra ZONOS2 MoE) through staged preprocessing → AR-decode → vocoder pipelines
- Initiated a codebase-wide refactor of the TTS serving stack, proposing migration of the last bespoke-scheduler AR model (~591-line custom scheduler) onto the shared scheduler used by every other model
- Optimized model serving via torch.compile + CUDA Graph capture (22ms → 4ms per-frame decode latency), a content-keyed LRU cache for reference-audio encoding (3x latency cut), and radix-cache adaptation for multi-channel token sequences to reuse cached reference-audio prefixes

**Microsoft Research Asia** (Jul 2024 - Jul 2025)
*Research Intern, Systems & Networking Group*
Mentored by [Dr. Li Lyna Zhang](https://www.microsoft.com/en-us/research/people/lzhani/)

- Led [**LoongRL**](https://arxiv.org/abs/2510.19363): Novel data synthesis + reinforcement learning enabling 7B models to surpass 32B LRMs in long-context reasoning (100k-200k tokens) (**ICLR 2026 Oral**)
- Contributed to [**LongRoPE2**](https://arxiv.org/abs/2502.20082): Extended LLM context windows to 128K tokens while retaining 98.5% short-context accuracy (**ICML 2025 poster**)
- Built parallel pipeline for large-scale user-query processing; delivered production-ready long-context recommendation models to [Microsoft Asia-Pacific R&D](https://www.microsoft.com/en-us/aprd/default)

**Carnegie Mellon University** (Oct 2025 – Present)
*Research Assistant, Language Technologies Institute*

- Synthetic task generation for training coding agents to generalize across repository-level environments ([Hybrid-Gym](https://arxiv.org/abs/2602.16819v1), **ICML 2026**)

**University of Illinois Urbana-Champaign**
*Research Assistant* with [Prof. Fan Lai](https://www.fanlai.me/) and [Prof. Minjia Zhang](https://minjiazhang.github.io/)

- Monte-Carlo-Tree-Search planning for cost-efficient LLM training on heterogeneous GPUs/TPUs
- Robustness benchmarking of LLMs ([Stochastic Monkeys](https://arxiv.org/abs/2411.02785))

---

### Research Interests

- Long-context reasoning & scaling
- Reinforcement learning for LLMs
- Efficient training architectures
- Code generation agents

---

### Beyond Research

Outside work, I enjoy gaming (lifetime **Faker** fan), vibe to rap, and hunt for the perfect **omakase** bite.

*Feel free to reach out - always happy to connect with like-minded friends and collaborators!*
