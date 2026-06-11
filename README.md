# Awesome Music Agent Skills [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of the best tools, APIs, libraries, MCP servers, and resources for building music-related AI agent skills — covering generation, analysis, transcription, stem separation, recommendation, and more.

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.

---

## Contents

- [Music Generation](#music-generation)
- [Music Analysis & MIR](#music-analysis--mir)
- [Transcription & Score Recognition](#transcription--score-recognition)
- [Stem Separation & Source Separation](#stem-separation--source-separation)
- [Music Recommendation & Discovery](#music-recommendation--discovery)
- [Open Source Libraries](#open-source-libraries)
- [APIs for Developers](#apis-for-developers)
- [MCP Servers (Model Context Protocol)](#mcp-servers-model-context-protocol)
- [Portable Music Agents & Skills](#portable-music-agents--skills)
- [Music Psychology & State-Change Research](#music-psychology--state-change-research)
- [DAW Plugins & Creative Tools](#daw-plugins--creative-tools)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Related Awesome Lists](#related-awesome-lists)

---

## Music Generation

AI-powered tools and models for generating music from text, MIDI, or other inputs.

- **[Suno AI](https://suno.com)** – Text-to-music generator producing full songs with vocals; leading platform for high-quality, instant track creation.
- **[Udio](https://www.udio.com)** – Studio-quality AI music generation with detailed style and genre control; strong for extended, editable compositions.
- **[AIVA](https://www.aiva.ai)** – AI composer focused on orchestral and cinematic music; supports MIDI export and DAW integration.
- **[Boomy](https://boomy.com)** – Quick music generation and publishing; beginner-friendly with commercial distribution.
- **[Soundraw](https://soundraw.io)** – Royalty-free AI music generation by mood, genre, and length; designed for content creators.
- **[Mubert](https://mubert.com)** – Generative streaming music via API; text-to-music and mood-based generation at scale.
- **[Riffusion](https://github.com/riffusion/riffusion)** — Real-time music generation using stable diffusion on spectrogram images; open source. `Python`
- **[Audiocraft / MusicGen](https://github.com/facebookresearch/audiocraft)** — Meta's open-source framework including MusicGen (text-to-music) and AudioGen (sound effects). `Python`
- **[Magenta](https://github.com/magenta/magenta)** — Google's research project using ML for music and art generation; includes RNN, VAE, and Transformer models. `Python`
- **[musiclm-pytorch](https://github.com/lucidrains/musiclm-pytorch)** — Unofficial PyTorch implementation of Google's MusicLM architecture. `Python`
- **[AudioLDM2](https://github.com/haoheliu/AudioLDM2)** — Latent diffusion model for high-quality text-to-audio and text-to-music generation. `Python`
- **[Stable Audio](https://www.stableaudio.com)** — Stability AI's text-to-audio platform; generates high-fidelity audio up to 3 minutes. API available.
- **[YuE](https://github.com/multimodal-art-projection/YuE)** — Open foundation model for full-song generation (vocals + instruments) from lyrics and style prompts. `Python`
- **[ElevenLabs Music](https://elevenlabs.io/music)** — High-quality modular AI music and sound design generation from ElevenLabs.
- **[BandLab SongStarter](https://www.bandlab.com/songstarter)** — Instant AI-generated chord and instrumental ideas to kick-start a song.

## Music Analysis & MIR

Music Information Retrieval (MIR) tools for extracting structure, key, tempo, chords, and other features from audio.

- **[librosa](https://github.com/librosa/librosa)** — The de-facto Python library for audio analysis: MFCCs, chroma, beat tracking, spectral features, pitch detection. `Python`
- **[Essentia](https://github.com/MTG/essentia)** — C++/Python library from MTG for comprehensive audio analysis and MIR; includes real-time processing and genre/key/mood classifiers. `C++` `Python`
- **[Sonoteller](https://sonoteller.ai)** — Cloud API for deep song analysis: mood, genre, tempo, lyrics structure, and music metadata.
- **[Cyanite](https://cyanite.ai)** — AI-powered music analysis and similarity search API; mood, genre, and energy tagging for large catalogs.
- **[AcousticBrainz](https://acousticbrainz.org)** — Open community-driven database of music audio features extracted with Essentia. (Dataset)
- **[madmom](https://github.com/CPJKU/madmom)** — Python audio and music signal processing library with strong beat/downbeat tracking models. `Python`
- **[aubio](https://github.com/aubio/aubio)** — C library with Python bindings for onset detection, pitch tracking, tempo analysis, and beat tracking. `C` `Python`
- **[Chroma.js / Pitchfork](https://github.com/neilgupta/Chroma)** — JavaScript chroma vector and key detection for in-browser music analysis. `JavaScript`
- **[mir_eval](https://github.com/craffel/mir_eval)** — Python library for evaluating common MIR tasks (beat tracking, chord estimation, melody extraction). `Python`

## Transcription & Score Recognition

Tools for converting audio to MIDI, sheet music, or symbolic notation.

- **[Basic Pitch](https://github.com/spotify/basic-pitch)** — Spotify's lightweight, open-source audio-to-MIDI transcription model; runs in browser, Python, and JS. `Python` `JavaScript`
- **[Piano Transcription](https://github.com/bytedance/piano_transcription)** — ByteDance high-quality piano audio-to-MIDI transcription system. `Python`
- **[Omnizart](https://github.com/Music-and-Culture-Technology-Lab/omnizart)** — Omnidirectional music transcription library covering piano, drums, chord, and vocal melody. `Python`
- **[Oemer](https://github.com/BreezeWhite/oemer)** — End-to-end optical music recognition (OMR) that converts sheet music images to MusicXML. `Python`
- **[music21](https://github.com/cuthbertLab/music21)** — MIT toolkit for computational musicology; parses MusicXML, MIDI, ABC notation; harmonic and counterpoint analysis. `Python`
- **[Moises](https://moises.ai)** — Real-time chord, beat, and melody transcription with an accessible developer API.
- **[PianoScribe](https://github.com/LostPolygon/piano-scribe)** — Lightweight piano transcription focused on producing clean, readable sheet music output. `Python`

## Stem Separation & Source Separation

Extract individual instruments or vocals from mixed audio.

- **[Demucs](https://github.com/facebookresearch/demucs)** — Meta's state-of-the-art waveform-based source separation model (4–6 stems); widely used in production. `Python`
- **[Spleeter](https://github.com/deezer/spleeter)** — Deezer's fast 2/4/5-stem separator; easy CLI and Python API. `Python`
- **[Open-Unmix (UMX)](https://github.com/sigsep/open-unmix-pytorch)** — Reference implementation for music source separation; well-documented and extensible. `Python`
- **[LALAL.AI](https://www.lalal.ai)** — Commercial cloud service for high-quality stem separation; REST API available.
- **[Moises Stem Splitter](https://moises.ai)** — API-accessible stem separation alongside chord/beat detection.
- **[AudioSep](https://github.com/Audio-AGI/AudioSep)** — Universal sound separation guided by natural language queries ("separate the guitar"). `Python`

## Music Recommendation & Discovery

Engines and APIs for music recommendation, mood detection, and playlist curation.

- **[Cyanite](https://cyanite.ai)** — Semantic music similarity search API; powers smart playlist curation and mood-based discovery.
- **[Sonoteller](https://sonoteller.ai)** — Deep audio analysis with mood, genre, energy, and structure tagging for recommendation pipelines.
- **[AudD](https://audd.io)** — Music recognition (like Shazam) API; identify songs from audio snippets programmatically.
- **[Acoustid](https://acoustid.org)** — Open-source audio fingerprinting API for music identification using the Chromaprint library.
- **[Chromaprint](https://github.com/acoustid/chromaprint)** — Fast acoustic fingerprint algorithm and library; core of Acoustid. `C`
- **[Beets](https://github.com/beetbox/beets)** — Extensible music library manager with auto-tagging, duplicate detection, and plugin architecture. `Python`
- **[spotipy](https://github.com/spotipy-dev/spotipy)** — Lightweight Python wrapper for the Spotify Web API; access track metadata, recommendations, and audio features. `Python`

## Open Source Libraries

Foundational Python and JS libraries for building music agent skills.

- **[librosa](https://github.com/librosa/librosa)** — Audio analysis and feature extraction. `Python`
- **[Essentia](https://github.com/MTG/essentia)** — Comprehensive MIR and audio analysis. `C++` `Python`
- **[music21](https://github.com/cuthbertLab/music21)** — Symbolic music analysis and generation (MIDI, MusicXML). `Python`
- **[pretty_midi](https://github.com/craffel/pretty-midi)** — Simple, pythonic MIDI file read/write and manipulation. `Python`
- **[mido](https://github.com/mido/mido)** — Low-level MIDI message and file library; real-time MIDI I/O. `Python`
- **[pyfluidsynth](https://github.com/nwhitehead/pyfluidsynth)** — Python bindings for FluidSynth; MIDI synthesizer for rendering soundfonts. `Python`
- **[pedalboard](https://github.com/spotify/pedalboard)** — Spotify's Python/NumPy library for audio effects (reverb, EQ, compression) using VST3/AU plugins. `Python`
- **[Tone.js](https://github.com/Tonejs/Tone.js)** — Web Audio API framework for creating interactive music and synthesis in the browser. `JavaScript`
- **[jsmidgen](https://github.com/dingram/jsmidgen)** — Node.js MIDI file writer; easy programmatic MIDI generation. `JavaScript`
- **[mingus](https://github.com/bspaans/python-mingus)** — Music theory and MIDI playback library with chord/scale/progression tools. `Python`
- **[pyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis)** — Audio feature extraction, classification, segmentation, and visualization toolkit. `Python`

## APIs for Developers

Hosted services with REST/WebSocket APIs for integrating music capabilities into agents.

| Service | Key Capabilities | Notes |
|---|---|---|
| **[Suno API](https://suno.com)** | Text-to-song, vocals, style control | Commercial; widely used |
| **[MusicGPT API](https://musicgpt.com/api)** | Generation, remixing, stem split, voice clone, 140+ TTS languages | Enterprise-scale |
| **[MusicAI API](https://music.ai/platform/api/)** | 50+ modules: stem sep, transcription, voice detection, metadata | One-stop audio pipeline |
| **[Mureka API](https://www.mureka.ai)** | Full song generation, vocal synthesis, audio analysis | Agent-studio included |
| **[Moises API](https://moises.ai/developers)** | Transcription, stem separation, mastering, chord/beat analysis | Strong for music learning apps |
| **[Mubert API](https://mubert.com/render/api)** | Text-to-music streaming, mood-based generation | Real-time generation |
| **[AudD API](https://audd.io)** | Song recognition from audio, lyrics, metadata | High accuracy fingerprinting |
| **[Acoustid API](https://acoustid.org/webservice)** | Audio fingerprint lookup | Open source backend |
| **[Spotify Web API](https://developer.spotify.com/documentation/web-api)** | Audio features, recommendations, catalog search | OAuth, broad catalog |
| **[Cyanite API](https://cyanite.ai/developers)** | Similarity search, mood/genre tagging, playlist curation | GraphQL |

## MCP Servers (Model Context Protocol)

MCP servers let AI agents (Claude, Copilot, etc.) interact with music services through standardized tool calls.

- **[youtube-music-mcp-server](https://github.com/mondweep/youtube-music-mcp-server)** — MCP server for searching and playing YouTube Music via Chrome automation; supports `search_song` and `play_song` tools.
- **[spotify-mcp](https://github.com/varunneal/spotify-mcp)** — MCP server exposing Spotify playback controls and search to AI agents (play, pause, search, queue).
- **[vibe-os MCP server](https://github.com/frankxai/vibe-os)** — MCP server for the vibe-os state-change music engine (`mcp-server/server.py`); 7 tools covering vibe-state listing, state/transition/custom prompt generation, frequency presets, frequency session design with WAV rendering, and session mix planning. `Python`
- **[MCP Registry](https://github.com/modelcontextprotocol/registry)** — Official registry for discovering MCP servers across all categories including music and media.
- **[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)** — Reference implementations and a growing collection of community MCP servers.
- **[MCPList.ai](https://mcplist.ai)** — Directory of verified MCP servers with music and media categories.

> **Building your own?** Use the official [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) or [TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) to wrap any music API as an MCP tool your agent can call.

## Portable Music Agents & Skills

Ready-made music agent definitions and skills you can load into Claude Projects, Custom GPTs, Gemini Gems, or any agent runtime.

- **[ai-music-academy portable agents](https://github.com/frankxai/ai-music-academy)** — Music education agents at `agents/portable/`, paired with a 4-tier curriculum from first prompt to professional production.
- **[claude-skills-library Suno skills](https://github.com/frankxai/claude-skills-library)** — Free Claude Code skills for AI music production: `suno-ai-mastery` (genre-specific Suno production patterns) and `suno-prompt-architect` (professional prompt design with style stacking).
- **[music-intelligence-systems](https://github.com/frankxai/music-intelligence-systems)** — Hub and registry of ~30 music agents across the FrankX ecosystem; JSON schemas plus portable exports for Claude Projects, Custom GPTs, Gemini Gems, and generic system prompts. Includes Lyric Writer, Film/Sync Composer, Music Theory Teacher, and Orchestration Architect agents.
- **[Starlight sound-intelligence vertical](https://github.com/frankxai/Starlight-Intelligence-System)** — Public reference vertical at `verticals/sound-intelligence/`: 6 sub-systems and 30 `/sound-*` commands spanning composition, production, performance, catalog, sync, and audience.
- **[vibe-os skills](https://github.com/frankxai/vibe-os)** — State-change music skills at `skills/<name>/SKILL.md`, built on a 15-state library and frequency tools; research-backed tempo/mode/timbre parameters in portable SKILL.md format.

## Music Psychology & State-Change Research

Research documentation grounding music agents in published psychology and acoustics findings.

- **[Frequency Healing Research](https://github.com/frankxai/vibe-os/blob/main/docs/frequency-healing-research.md)** — Evidence review of frequency-based audio (binaural beats, entrainment); separates supported effects from marketing claims.
- **[Music Psychology Research](https://github.com/frankxai/vibe-os/blob/main/docs/music-psychology-research.md)** — Annotated research notes on tempo, mode, timbre, and lyrics effects used by the vibe-os engine.
- **[music-intelligence-systems research](https://github.com/frankxai/music-intelligence-systems)** — Music-psychology research framework at `research/`: shared methodology plus an open-questions registry for cross-agent studies.
- **[The Science of State-Change (whitepaper)](https://github.com/frankxai/vibe-os/blob/main/docs/whitepaper-the-science-of-state-change.md)** — vibe-os whitepaper on designing music for deliberate state change; grounds the 15-state library in cited studies.

## DAW Plugins & Creative Tools

AI plugins that bring agent-like intelligence into Digital Audio Workstations.

- **[Magenta Studio](https://magenta.tensorflow.org/studio)** — Ableton Live plugins (Continue, Generate, Groove, Interpolate, Drumify) powered by Google Magenta models.
- **[ORB Producer Suite 3](https://www.orbplugins.com)** — AI MIDI chord progressions, basslines, and melody generation as VST/AU DAW plugins.
- **[iZotope Neutron](https://www.izotope.com/en/products/neutron.html)** — AI-assisted mixing with intelligent EQ and compression suggestions.
- **[iZotope Ozone](https://www.izotope.com/en/products/ozone.html)** — AI mastering assistant with reference matching and loudness targeting.
- **[LANDR Studio](https://www.landr.com)** — Cloud-based AI mastering, distribution, and sample library.
- **[Sonible Smart:EQ](https://www.sonible.com/smarteq4/)** — Machine-learning EQ that profiles your mix and applies intelligent corrections.
- **[Dreamtonics Synthesizer V](https://dreamtonics.com/synthesizerv/)** — AI vocal synthesis engine for singing voice generation inside DAWs.
- **[Samplab](https://samplab.com)** — AI-powered sample manipulation: pitch-shift individual notes and remix drum loops.

## Datasets & Benchmarks

Open datasets for training and evaluating music agent models.

- **[MagnaTagATune](https://mirg.city.ac.uk/codeapps/the-magnatagatune-dataset)** — 25,000 audio clips with multi-label tags for music auto-tagging.
- **[FMA (Free Music Archive)](https://github.com/mdeff/fma)** — 106,574 tracks with metadata for music genre classification. `Python`
- **[MAESTRO](https://magenta.tensorflow.org/datasets/maestro)** — 200+ hours of aligned piano MIDI and audio for transcription research.
- **[GTZAN](https://marsyasweb.appspot.com/download/data_sets/)** — Classic 10-genre music classification benchmark (1,000 audio clips).
- **[MusicCaps](https://www.kaggle.com/datasets/googleai/musiccaps)** — Google's 5,500 music clips with expert text captions; key benchmark for text-to-music models.
- **[MTG-Jamendo](https://github.com/MTG/mtg-jamendo-dataset)** — 55,000 tracks with mood, genre, and instrument tags from Jamendo. `Python`
- **[Slakh2100](http://www.slakh.com)** — 2,100 multi-track MIDI-audio pairs for source separation and transcription.
- **[NSynth](https://magenta.tensorflow.org/nsynth)** — 300,000 musical notes from 1,000 instruments with rich annotations.

---

## Related Awesome Lists

- [Curated-Awesome-Lists/awesome-ai-music-generation](https://github.com/Curated-Awesome-Lists/awesome-ai-music-generation) — Deep dive into AI generative music research, papers, and projects.
- [steven2358/awesome-music-ai](https://github.com/steven2358/awesome-music-ai) — Broad curated list of AI tools for music composition, generation, and analysis.
- [phobal/awesome-music](https://github.com/phobal/awesome-music) — General awesome list of music libraries, tools, and frameworks.
- [ciconia/awesome-music](https://github.com/ciconia/awesome-music) — Curated list of music tools spanning notation, audio, MIDI, and theory.
- [josephmisiti/awesome-machine-learning](https://github.com/josephmisiti/awesome-machine-learning#speech) — Speech and audio section of the master ML awesome list.

---

## Contributing

1. Fork the repository.
2. Add your resource under the appropriate category, following the existing format.
3. Ensure the link is working and the description is concise.
4. Submit a pull request.

Please keep entries focused on **agent-usable** skills — APIs, libraries, models, and tools that can be called programmatically by an AI agent.

---

*Maintained by [@frankxai](https://github.com/frankxai). Last updated June 2026.*