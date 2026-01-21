<p align="center">
  <img src="https://raw.githubusercontent.com/simple-eiffel/.github/main/profile/assets/logo.png" alt="Simple Eiffel" width="300">
</p>

# Simple Eiffel

**114 production-ready Eiffel libraries for modern software development**

[![Libraries](https://img.shields.io/badge/libraries-114-blue)](https://github.com/simple-eiffel)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Eiffel](https://img.shields.io/badge/Eiffel-25.02-orange)](https://www.eiffel.org/)

---

## What is New (January 2026) — 22 libraries

### Template & Code Generation
- **simple_template** *(Dec 6 + Jan)* - Mustache + Evolicity directives, expression evaluator, filters, compiled templates (116 tests)
- **simple_code** *(Jan 14)* - AI-assisted code generation with Inno Setup builder

### Data & Persistence
- **simple_persist** *(Jan 20)* - SCOOP-safe object persistence with contracts
- **simple_zstring** *(Jan 19)* - Unicode strings with Eiffel-Loop integration (182 tests)
- **simple_container** *(Jan 20)* - LINQ-style collection operations (51 tests)
- **simple_sorter** *(Jan 20)* - Sorting algorithms integrated into simple_math

### Testing & Development
- **simple_mock** *(Jan 18)* - HTTP mock server for integration testing (34 tests)
- **simple_diff** *(Jan 18)* - Myers diff algorithm (19 tests)
- **simple_reflection** *(Jan 19)* - Runtime introspection (36 tests)
- **simple_factory** *(Jan 19)* - Object factory patterns (53 tests)
- **simple_encoding** *(Jan 19)* - Character encoding detection v2.0.0 (83 tests)

### Graphics (Experimental)
- **simple_vulkan** *(Jan 15)* - Vulkan graphics API bindings
- **simple_sdf** *(Jan 15)* - Signed distance field rendering
- **simple_shaderc** *(Jan 15)* - Shader compilation

*January effort: ~220 hours over 20 days (includes work on Vox and other personal Eiffel projects)*

---

## December 2025 — 87 libraries (The Expansion)

### Core Data Formats
- **simple_csv** *(Dec 5)* - RFC 4180 CSV parsing with streaming
- **simple_xml** *(Dec 6)* - XML parsing with XPath support
- **simple_yaml** *(Dec 10)* - YAML 1.2 parser
- **simple_toml** *(Dec 10)* - TOML configuration files
- **simple_markdown** *(Dec 6)* - Markdown to HTML conversion

### Web & Networking
- **simple_http** *(Dec 7)* - HTTP client with Win32 WinHTTP
- **simple_websocket** *(Dec 6)* - WebSocket client/server
- **simple_smtp** *(Dec 5)* - Email sending
- **simple_grpc** *(Dec 13)* - gRPC protocol support

### Security & Auth
- **simple_jwt** *(Dec 5)* - JWT token creation/validation
- **simple_encryption** *(Dec 7)* - AES, RSA, hashing via Win32 CNG
- **simple_hash** *(Dec 5)* - SHA-256, MD5, HMAC
- **simple_base64** *(Dec 5)* - Base64 encoding/decoding
- **simple_uuid** *(Dec 5)* - UUID generation

### Data Storage
- **simple_cache** *(Dec 6)* - LRU cache + Redis client
- **simple_mq** *(Dec 13)* - Message queue abstraction
- **simple_registry** *(Dec 7)* - Windows registry access

### Device & Hardware
- **simple_ffmpeg** *(Dec 27)* - Video/audio transcoding via FFmpeg
- **simple_usb** *(Dec 27)* - USB/HID device access
- **simple_audio** *(Dec 27)* - Real-time audio I/O (WASAPI)
- **simple_serial** *(Dec 26)* - COM port communication
- **simple_bluetooth** *(Dec 26)* - Bluetooth SPP

### AI & Knowledge
- **simple_kb** *(Dec 24)* - Knowledge base with RAG search
- **simple_speech** *(Dec 28)* - Speaker diarization, AI correction
- **simple_rosetta** *(Dec 22)* - 273 Rosetta Code algorithms

### Developer Tools
- **simple_oracle** *(Dec 9)* - AI development memory/context system
- **simple_lsp** *(Dec 9)* - VS Code language server
- **simple_pkg** *(Dec 14)* - Package manager
- **simple_notebook** *(Dec 19)* - Interactive Eiffel REPL
- **simple_testing** *(Dec 7)* - Test framework
- **simple_eiffel_parser** *(Dec 10)* - Eiffel source parser
- **simple_cli** *(Dec 7)* - Command-line argument parsing
- **simple_console** *(Dec 7)* - Terminal colors and formatting
- **simple_env** *(Dec 7)* - Environment variable management
- **simple_config** *(Dec 7)* - Configuration file handling
- **simple_logger** *(Dec 6)* - Structured logging

### Infrastructure
- **simple_docker** *(Dec 16)* - Docker container management
- **simple_k8s** *(Dec 17)* - Kubernetes orchestration
- **simple_scheduler** *(Dec 13)* - Job scheduling, cron
- **simple_telemetry** *(Dec 13)* - Tracing and metrics

### Document Generation
- **simple_pdf** *(Dec 7)* - PDF generation with music notation
- **simple_cairo** *(Dec 29)* - 2D graphics, PDF surfaces

### Utilities
- **simple_file** *(Dec 6)* - File operations facade
- **simple_datetime** *(Dec 6)* - Date/time utilities
- **simple_regex** *(Dec 6)* - Regular expressions
- **simple_validation** *(Dec 6)* - Input validation
- **simple_archive** *(Dec 7)* - ZIP/TAR archive handling
- **simple_ipc** *(Dec 7)* - Inter-process communication
- **simple_mmap** *(Dec 7)* - Memory-mapped files
- **simple_fraction** *(Dec 11)* - Rational number arithmetic
- **simple_decimal** *(Dec 11)* - Decimal number support
- **simple_math** *(Dec 13)* - Mathematical functions
- **simple_graph** *(Dec 13)* - Graph data structures

*December effort: ~330 hours over 30 days*

---

## November 2025 — 5 libraries (The Founding)

The Simple Eiffel ecosystem began on **November 11, 2025** with the creation of simple_json.

- **simple_json** *(Nov 11)* - JSON parser with Schema, Patch, Pointer support - **the first library**
- **simple_web** *(Nov 21)* - Web framework with routing and middleware
- **simple_sql** *(Nov 22)* - SQLite database with fluent query API
- **simple_ai_client** *(Nov 23)* - Multi-provider AI client (OpenAI, Anthropic, Google, Ollama)

*November effort: ~130 hours over 12 days*

---

## Ecosystem Totals

| Period | Libraries | Hours | Days |
|--------|-----------|-------|------|
| November 2025 | 5 | ~130h | 12 |
| December 2025 | 87 | ~330h | 30 |
| January 2026 | 22 | ~220h | 20 |
| **Total** | **114** | **~680h** | **71** |

*Built collaboratively by Larry Rix and Claude (Anthropic) — Human+AI development*

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

### Recently Updated

| Library | Description | Tests |
|---------|-------------|-------|
| [simple_template](https://github.com/simple-eiffel/simple_template) | Mustache + Evolicity directives, compiled templates | 116 |
| [simple_persist](https://github.com/simple-eiffel/simple_persist) | SCOOP-safe object persistence | 24 |
| [simple_zstring](https://github.com/simple-eiffel/simple_zstring) | Unicode strings (Eiffel-Loop integration) | 182 |
| [simple_container](https://github.com/simple-eiffel/simple_container) | LINQ-style collection operations | 51 |
| [simple_mock](https://github.com/simple-eiffel/simple_mock) | HTTP mock server for testing | 34 |
| [simple_diff](https://github.com/simple-eiffel/simple_diff) | Myers diff algorithm | 19 |

### AI & Speech

| Library | Description | Tests |
|---------|-------------|-------|
| [simple_ai_client](https://github.com/simple-eiffel/simple_ai_client) | OpenAI, Anthropic, Google, Ollama | 12 |
| [simple_speech](https://github.com/simple-eiffel/simple_speech) | Speaker diarization, AI correction | 6 |

### Device Libraries

| Library | Description | Tests |
|---------|-------------|-------|
| [simple_ffmpeg](https://github.com/simple-eiffel/simple_ffmpeg) | Video/audio transcoding, metadata | 19 |
| [simple_usb](https://github.com/simple-eiffel/simple_usb) | USB/HID devices, gamepads | 29 |
| [simple_audio](https://github.com/simple-eiffel/simple_audio) | Real-time audio I/O (WASAPI) | 17 |
| [simple_serial](https://github.com/simple-eiffel/simple_serial) | COM port communication | 6 |
| [simple_bluetooth](https://github.com/simple-eiffel/simple_bluetooth) | Bluetooth SPP | 11 |

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

*114 libraries. One ecosystem. Modern Eiffel.*
