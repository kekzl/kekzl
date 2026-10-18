# Hey, I'm Raph

I build AI tools and many more.

## 🔥 What I'm building right now: imp

[![imp](https://img.shields.io/badge/kekzl/imp-181717?style=flat&logo=github&logoColor=white)](https://github.com/kekzl/imp)
[![Stars](https://img.shields.io/github/stars/kekzl/imp?style=flat&color=yellow)](https://github.com/kekzl/imp/stargazers)
![CUDA](https://img.shields.io/badge/CUDA-13.4-76b900?style=flat&logo=nvidia)
![C++23](https://img.shields.io/badge/C%2B%2B-23-00599C?style=flat&logo=cplusplus)
![License](https://img.shields.io/github/license/kekzl/imp?style=flat&color=blue)

A **from-scratch C++/CUDA LLM server for one GPU generation**: the RTX 5090 / RTX PRO 6000 (`sm_120a`), with native FP4 math. No wrapper around llama.cpp or vLLM. One `docker run`, OpenAI and Anthropic API, tool calling, JSON output, thinking models, built-in chat. ~346k lines, every one written by [Claude Code](https://claude.ai/claude-code).

**Qwen3.8-27B on one RTX 5090**, each engine on its defaults:

| | **imp** | vLLM 0.31.0 | llama.cpp |
| --- | ---: | ---: | ---: |
| one user | **91.0-93.7 tok/s** | 68.9-70.0 tok/s | 61.8-63.0 tok/s |
| 32 users at once (total) | **1963.5-1977.0 tok/s** | 1354.8-1449.4 tok/s | 162.0-166.8 tok/s |

- 🚀 **Qwen3.8-Flash-Next:** 123.6 GiB checkpoint on a 32 GB card, experts in host RAM, **87.89-98.57 tok/s**
- 🎯 **Same GGUF as llama.cpp:** **72.7-73.4** vs 60.5-61.0 tok/s for one user, **240.0-244.4** vs 154.5-155.1 for 32 users

Every number measured, dated and commit-anchored: **[github.com/kekzl/imp](https://github.com/kekzl/imp)**

## Other things I build

**GPU & AI**

- **[apa](https://github.com/kekzl/apa)**: adaptive-precision attention prefill for `sm_120a`: FP4 pass plus exact FP16 hot tiles.
- **[cplusplus-cuda-graph](https://github.com/kekzl/cplusplus-cuda-graph)**: recovers CUDA launch and destructor edges for CodeGraph. On imp: kernel launch coverage 74.2% → 99.3%.
- **[axo](https://github.com/kekzl/axo)**: continually learning spiking neural network in C++23/CUDA, local plasticity (STDP, R-STDP) instead of backprop.
- **[guilty-until-proven](https://github.com/kekzl/guilty-until-proven)**: operating manual for a Claude Code session that drives other sessions and rejects anything without evidence.
- **[PromptMill](https://github.com/kekzl/PromptMill)**: local-first prompt generator, 132 roles for video, image, audio and 3D models. Offline, auto-scaled to your VRAM.

**Infrastructure & tools**

- **[entra-id-secrets-notification](https://github.com/kekzl/entra-id-secrets-notification)**: alerts on expiring Entra ID secrets and certificates via Teams, Slack, Email or Webhook.
- **[mailcow-ai-filter](https://github.com/kekzl/mailcow-ai-filter)**: AI email sorting for MailCow, generates Sieve filters with Claude or local LLMs.
- **[MeetingRoomUsageAnalyzer](https://github.com/kekzl/MeetingRoomUsageAnalyzer)**: meeting room usage via Microsoft Graph, React + FastAPI dashboard.
- **[dns-speedtester](https://github.com/kekzl/dns-speedtester)**: finds the fastest DNS resolver from your location, stdlib Python in a container.
- **[bienchen](https://github.com/kekzl/bienchen)**: a honeybee flying through a summer meadow, real-time WebGL2, no build step.

## Stack

**Infrastructure** · `VMware vSphere` `NetApp` `OpenZFS` `Linux` `Docker` `Ansible` `Entra ID` `Microsoft 365`

**AI / ML** · `CUDA` `C++23` `NVFP4` `LLM Inference` `LLM Pretraining` `Claude Code`

## Interests

Custom Water Cooling · PC Building · Home Automation · AI Video Generation · Stock Market · Skiing

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raphael-friedmann-a0617213b/)
