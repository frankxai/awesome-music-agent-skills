# Awesome Music Agent Skills

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Link Check](https://github.com/frankxai/awesome-music-agent-skills/actions/workflows/link-checker.yml/badge.svg)](https://github.com/frankxai/awesome-music-agent-skills/actions/workflows/link-checker.yml)

> A **web-first** catalog of music generation, audio analysis, composition, and agent-skill resources.  
> Useful even if every frankxai link is removed.

**Research pulse:** 2026-08-07  
**Maturity labels:** production · beta · experimental · reference

This list is a **catalog**, not a runtime. For a working Hermes music producer distribution see [`agentic-music-producer-os`](https://github.com/frankxai/agentic-music-producer-os) (optional).

---

## Contents

- [Official platforms & docs](#official-platforms--docs)
- [Open-source audio / music models](#open-source-audio--music-models)
- [Agent skills & MCP](#agent-skills--mcp)
- [Analysis, DSP, and datasets](#analysis-dsp-and-datasets)
- [Prompts, structure, and craft](#prompts-structure-and-craft)
- [Related awesome lists](#related-awesome-lists)
- [Contributing](#contributing)

---

## Official platforms & docs

| Resource | Notes |
| --- | --- |
| [Suno](https://suno.com) | Hosted text-to-music product; describe musical attributes, not artist clones |
| [Udio](https://www.udio.com) | Hosted generation; check current ToS before automation |
| [AIVA](https://www.aiva.ai) | Composition assistant oriented to scoring workflows |
| [Stable Audio (Stability)](https://www.stableaudio.com) | Hosted + open-weight audio generation line |
| [Meta AudioCraft](https://github.com/facebookresearch/audiocraft) | MusicGen / AudioGen research code (production research stack) |
| [Google Magenta](https://magenta.tensorflow.org) | Long-running music+ML research and tools |

---

## Open-source audio / music models

| Project | Maturity | Notes |
| --- | --- | --- |
| [facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft) | production | MusicGen family; local/research generation |
| [ace-step/ACE-Step](https://github.com/ace-step/ACE-Step) | beta | Open music generation foundation model line |
| [OpenMusicLDM / AudioLDM ecosystem](https://github.com/haoheliu/AudioLDM2) | beta | Latent diffusion audio generation |
| [RVC-Project/Retrieval-based-Voice-Conversion-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | experimental | Voice conversion — high misuse risk; local only |
| [suno-ai/bark](https://github.com/suno-ai/bark) | reference | Historic generative audio; not the hosted Suno product API |

Prefer licenses + local isolation before any agent wiring. Do not treat stars as safety.

---

## Agent skills & MCP

| Project | Maturity | Notes |
| --- | --- | --- |
| [frankxai/agentic-music-producer-os](https://github.com/frankxai/agentic-music-producer-os) | beta | Hermes profile distribution for music production workflows |
| [frankxai/suno-mcp-server](https://github.com/frankxai/suno-mcp-server) | experimental | MCP surface for Suno-oriented flows — verify auth/ToS |
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | reference | Upstream MCP server patterns (general, not music-only) |
| [agentskills.io](https://agentskills.io) | reference | Cross-harness skill packaging conventions |

---

## Analysis, DSP, and datasets

| Project | Maturity | Notes |
| --- | --- | --- |
| [librosa/librosa](https://github.com/librosa/librosa) | production | Python audio analysis |
| [CPJKU/madmom](https://github.com/CPJKU/madmom) | production | Beat/onset/transcription oriented tools |
| [spotify/pedalboard](https://github.com/spotify/pedalboard) | production | Audio effects / processing in Python |
| [MTG/essentia](https://github.com/MTG/essentia) | production | Audio features and MIR library |
| [FMA: Free Music Archive dataset](https://github.com/mdeff/fma) | reference | Research dataset — respect licenses |

---

## Prompts, structure, and craft

| Practice | Why it matters for agents |
| --- | --- |
| Describe **genre, tempo, key, form, instrumentation, mix** | Avoids artist-name / voice-clone prompt patterns |
| Separate **lyrics**, **style tags**, and **arrangement** | Cleaner regeneration and edit loops |
| Keep a **listening test + version log** | Evidence > vibes when claiming improvement |
| Rights and platform ToS before publish | Generation ≠ distribution rights |

---

## Related awesome lists

| List | Focus |
| --- | --- |
| [ybayle/awesome-deep-learning-music](https://github.com/ybayle/awesome-deep-learning-music) | Academic deep learning + music |
| [shuyaoliu/awesome-ai-music](https://github.com/shuyaoliu/awesome-ai-music) | Broader AI music links |
| [frankxai/awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) | Hermes-compatible skills (optional) |

---

## Contributing

1. Prefer **source-verified** upstream links (repo, docs, or paper).
2. Add a short annotation and a maturity label.
3. No funnel-only READMEs, no paywalled-only entries without a free primary source.
4. Do not add artist-clone, voice-theft, or ToS-violating automation recipes.
5. Open a PR; keep edits web-first and useful without frankxai links.

---

## Maintainer note

Historical Hub-and-Spoke CTA stubs were removed on 2026-08-07. Stars and Gumroad links are not evidence. Runtime music production for Hermes lives in `agentic-music-producer-os`, not this catalog.
