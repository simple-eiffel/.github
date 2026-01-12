<p align="center">
  <img src="https://raw.githubusercontent.com/simple-eiffel/.github/main/profile/assets/logo.png" alt="Simple Eiffel" width="300">
</p>

# Simple Eiffel

**85+ production-ready Eiffel libraries for modern software development**

[![Libraries](https://img.shields.io/badge/libraries-85+-blue)](https://github.com/simple-eiffel)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Eiffel](https://img.shields.io/badge/Eiffel-25.02-orange)](https://www.eiffel.org/)

---

## What is New (January 2026)

### Speech & AI Libraries
- **simple_speech** - Speaker diarization, AI semantic correction, SRT/VTT exports with AI metadata
- **simple_ai_client** - Google AI provider support, OpenAI improvements, environment variable handling

### Document Generation
- **simple_pdf** - Native music notation PDF rendering module (notes, rests, time signatures)
- **simple_cairo** - PDF surface support for vector graphics output

### Developer Tools
- **simple_kb** - AI-enhanced knowledge base with 4-phase RAG (182 libraries, 87K features indexed)
- **simple_notebook** - Interactive Eiffel REPL with multi-class + multiple inheritance
- **simple_pkg** - Package manager for the ecosystem

### Device Libraries
- **simple_ffmpeg** - FFmpeg multimedia: transcoding, metadata, extraction (CLI + SDK modes)
- **simple_usb** - USB/HID device access, gamepads, Arduino detection
- **simple_audio** - Real-time audio I/O via WASAPI, PCM buffers
- **simple_serial** - COM port communication
- **simple_bluetooth** - Bluetooth SPP communication

---

## Quick Start

### Windows

1. Install [EiffelStudio 25.02](https://www.eiffel.org/downloads)
2. Set environment variable: `setx SIMPLE_EIFFEL D:\path\to\simple_eiffel`
3. Add to your ECF:
   ```xml
   <library name="simple_json" location="$SIMPLE_EIFFEL/simple_json/simple_json.ecf"/>
   ```

### Package Manager

```bash
simple_pkg install simple_json
simple_pkg install all     # Install entire ecosystem
```

---

## Featured Libraries

### Speech & AI (NEW!)

| Library | Description | Tests |
|---------|-------------|-------|
| [simple_speech](https://github.com/simple-eiffel/simple_speech) | Speaker diarization, AI correction | 6/6 |
| [simple_ai_client](https://github.com/simple-eiffel/simple_ai_client) | OpenAI, Anthropic, Google, Ollama | 12/12 |

### Device Libraries

Hardware and multimedia access with Design by Contract:

| Library | Description | Tests |
|---------|-------------|-------|
| [simple_ffmpeg](https://github.com/simple-eiffel/simple_ffmpeg) | Video/audio transcoding, metadata | 19/19 |
| [simple_usb](https://github.com/simple-eiffel/simple_usb) | USB/HID devices, gamepads | 29/29 |
| [simple_audio](https://github.com/simple-eiffel/simple_audio) | Real-time audio I/O (WASAPI) | 17/17 |
| [simple_serial](https://github.com/simple-eiffel/simple_serial) | COM port communication | 6/6 |
| [simple_bluetooth](https://github.com/simple-eiffel/simple_bluetooth) | Bluetooth SPP | 11/11 |

### simple_kb - AI Knowledge Base

Searchable Eiffel knowledge base with AI-enhanced RAG:
- **4,613 classes** and **87,780 features** indexed
- **31 compiler error codes** with causes and fixes
- **14 design patterns** with Eiffel idioms

```bash
kb search "void safety"
kb error VEVI
kb pattern singleton
```

### simple_rosetta - Algorithm Library

273 Rosetta Code solutions in Eiffel with contracts.

---

## Library Categories

### Data Formats
| Library | Description |
|---------|-------------|
| [simple_json](https://github.com/simple-eiffel/simple_json) | JSON with Schema, Patch, Pointer |
| [simple_csv](https://github.com/simple-eiffel/simple_csv) | RFC 4180 CSV parsing |
| [simple_xml](https://github.com/simple-eiffel/simple_xml) | XML parsing with XPath |
| [simple_yaml](https://github.com/simple-eiffel/simple_yaml) | YAML 1.2 parser |
| [simple_toml](https://github.com/simple-eiffel/simple_toml) | TOML configuration |

### Web and Networking
| Library | Description |
|---------|-------------|
| [simple_http](https://github.com/simple-eiffel/simple_http) | HTTP client |
| [simple_web](https://github.com/simple-eiffel/simple_web) | Web framework |
| [simple_websocket](https://github.com/simple-eiffel/simple_websocket) | WebSocket client/server |
| [simple_smtp](https://github.com/simple-eiffel/simple_smtp) | Email sending |
| [simple_grpc](https://github.com/simple-eiffel/simple_grpc) | gRPC protocol |

### Security and Auth
| Library | Description |
|---------|-------------|
| [simple_jwt](https://github.com/simple-eiffel/simple_jwt) | JWT tokens |
| [simple_encryption](https://github.com/simple-eiffel/simple_encryption) | AES, RSA, hashing |

### Data and Storage
| Library | Description |
|---------|-------------|
| [simple_sql](https://github.com/simple-eiffel/simple_sql) | SQLite with fluent API |
| [simple_cache](https://github.com/simple-eiffel/simple_cache) | LRU cache + Redis |
| [simple_mq](https://github.com/simple-eiffel/simple_mq) | Message queues |

### AI and Knowledge
| Library | Description |
|---------|-------------|
| [simple_kb](https://github.com/simple-eiffel/simple_kb) | Knowledge base with RAG |
| [simple_ai_client](https://github.com/simple-eiffel/simple_ai_client) | OpenAI, Anthropic, Google, Ollama |
| [simple_rosetta](https://github.com/simple-eiffel/simple_rosetta) | 273 algorithm implementations |

### Infrastructure
| Library | Description |
|---------|-------------|
| [simple_docker](https://github.com/simple-eiffel/simple_docker) | Container management |
| [simple_k8s](https://github.com/simple-eiffel/simple_k8s) | Kubernetes orchestration |
| [simple_scheduler](https://github.com/simple-eiffel/simple_scheduler) | Job scheduling, cron |
| [simple_telemetry](https://github.com/simple-eiffel/simple_telemetry) | Tracing, metrics |

### Developer Tools
| Library | Description |
|---------|-------------|
| [simple_lsp](https://github.com/simple-eiffel/simple_lsp) | VS Code language server |
| [simple_pkg](https://github.com/simple-eiffel/simple_pkg) | Package manager |
| [simple_notebook](https://github.com/simple-eiffel/simple_notebook) | Interactive Eiffel |
| [simple_testing](https://github.com/simple-eiffel/simple_testing) | Test framework |
| [simple_eiffel_parser](https://github.com/simple-eiffel/simple_eiffel_parser) | Eiffel source parser |

### Document Generation
| Library | Description |
|---------|-------------|
| [simple_pdf](https://github.com/simple-eiffel/simple_pdf) | PDF generation with music notation |
| [simple_cairo](https://github.com/simple-eiffel/simple_cairo) | 2D graphics, PDF surfaces |

---

## VS Code Integration

Install **Simple Eiffel LSP** from the VS Code marketplace:
- Syntax highlighting and Go to definition
- **DbC Heatmap** - Visualize contract coverage

---

## Design Principles

- **Design by Contract** - Preconditions, postconditions, invariants
- **Void Safety** - Compile-time null protection
- **SCOOP Compatible** - All libraries work with Eiffel concurrency
- **Human+AI Development** - Built collaboratively with Claude (Anthropic)

---

## Documentation

- **Website**: [simple-eiffel.github.io](https://simple-eiffel.github.io)
- **Each library**: `https://simple-eiffel.github.io/{library}/`

---

## Contributing

Issues and pull requests welcome. All code follows Design by Contract.

---

*85+ libraries. One ecosystem. Modern Eiffel.*
