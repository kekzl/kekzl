# Hey, I'm Raph

I run the IT infrastructure @ [EIFER — European Institute for Energy Research](https://www.eifer.org) and build AI tools on the side.

## 🔥 What I'm building right now — imp

[![imp](https://img.shields.io/badge/kekzl/imp-181717?style=flat&logo=github&logoColor=white)](https://github.com/kekzl/imp)
[![Stars](https://img.shields.io/github/stars/kekzl/imp?style=flat&color=yellow)](https://github.com/kekzl/imp/stargazers)
![CUDA](https://img.shields.io/badge/CUDA-13.3-76b900?style=flat&logo=nvidia)
![C++20](https://img.shields.io/badge/C%2B%2B-20-00599C?style=flat&logo=cplusplus)
![Status](https://img.shields.io/badge/status-experimental-orange?style=flat)

A **from-scratch C++/CUDA inference engine** that targets exactly one architecture: the NVIDIA RTX 5090 / RTX PRO 6000 (`sm_120a`). No portability layer, no wrapper around llama.cpp or vLLM — its own GGUF & SafeTensors loaders, BPE tokenizer, paged KV cache, attention/MoE kernels, Gated DeltaNet + Mamba2 scans, CUDA Graphs, and an OpenAI/Anthropic-compatible server built for **agentic AI**: tool calling, `json_schema` constrained decoding, separable reasoning channels and concurrent sub-agent fan-out.

The fastest single-GPU backend on the 5090 — and every line of its ~97k is written by [Claude Code](https://claude.ai/claude-code).

- ⚡ **GGUF dense decode:** Qwen3-8B Q8_0 at **~270 tok/s** — **+37–72% over llama.cpp**
- 🚀 **NVFP4 30B-class MoE decode:** **~257–338 tok/s** — uncontested on `sm_120` (vLLM's NVFP4 path needs `tcgen05`, absent on consumer Blackwell)
- 🎯 **NVFP4 long-context prefill:** at-or-ahead of vLLM (MoE pp4096 +4%, pp2048 +27%, TTFT wins everywhere)

Every number is measured, dated and commit-anchored → **[github.com/kekzl/imp](https://github.com/kekzl/imp)**

## Other things I build

- **[PromptMill](https://github.com/kekzl/PromptMill)** — AI prompt generator for video & image models (Wan2.1, FLUX, SD, Midjourney). Local LLMs with GPU auto-detection.
- **[mailcow-ai-filter](https://github.com/kekzl/mailcow-ai-filter)** — AI-powered email sorting for MailCow. Auto-generates Sieve filters using Claude or local LLMs.
- **[seedling](https://github.com/kekzl/seedling)** — Synthetic instruction dataset generator for SFT. Generate and curate training data with Ollama.
- **[entra-id-secrets-notification](https://github.com/kekzl/entra-id-secrets-notification)** — Monitor Azure AD secrets & certificates for expiration. Alerts via Teams, Slack, Email.
- **[mcp-docker-examples](https://github.com/kekzl/mcp-docker-examples)** — On-demand MCP servers using Docker Compose profiles.

## Stack

`CUDA` `C++20` `VMware vSphere` `NetApp` `OpenZFS` `Docker` `Linux` `Entra ID` `Microsoft 365` `Ansible` `Claude Code` `LLM Inference` `LLM Pretraining` `Penetration Testing`

## Interests

Custom Water Cooling · PC Building · Home Automation · AI Video Generation · Stock Market · Skiing

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raphael-friedmann-a0617213b/)
