<p align="center">
  <img src="https://raw.githubusercontent.com/simple-eiffel/claude_eiffel_op_docs/main/artwork/LOGO.png" alt="Simple Eiffel" width="300">
</p>

# Simple Eiffel

**75+ production-ready Eiffel libraries for modern software development**

[![Libraries](https://img.shields.io/badge/libraries-75+-blue)](https://github.com/simple-eiffel)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Eiffel](https://img.shields.io/badge/Eiffel-25.02-orange)](https://www.eiffel.org/)

---

## What is New (December 2024)

- **simple_kb** - AI-enhanced knowledge base with 4-phase RAG (182 libraries, 87K features indexed)
- **simple_gobo** - GitHub Gobo 2024 for SCOOP inline separate parsing
- **simple_rosetta** - 273 Rosetta Code algorithm implementations
- **simple_notebook** - Interactive Eiffel execution environment
- **QUICK APIs** - 17 libraries with zero-configuration beginner facades
- **simple_pkg** - Package manager for the ecosystem

---

## Quick Start

### Windows

1. Install [EiffelStudio 25.02](https://www.eiffel.org/downloads)
2. Set environment variable: `setx SIMPLE_EIFFEL D:\path\to\simple_eiffel`
3. Add to your ECF:
   ```xml
   <library name="simple_json" location="$SIMPLE_EIFFEL/simple_json/simple_json.ecf"/>
   ```

### Linux / WSL2

```bash
# Download EiffelStudio
wget https://ftp.eiffel.com/pub/download/25.02/Eiffel_25.02_rev_98732-linux-x86-64.tar.bz2
tar xjf Eiffel_25.02_rev_98732-linux-x86-64.tar.bz2

# Add to ~/.bashrc
export SIMPLE_EIFFEL=$HOME/simple_eiffel
export ISE_EIFFEL=$SIMPLE_EIFFEL/Eiffel_25.02
export ISE_PLATFORM=linux-x86-64
export PATH=$ISE_EIFFEL/studio/spec/$ISE_PLATFORM/bin:$PATH
```

### Package Manager

```bash
simple_pkg install simple_json
simple_pkg install all     # Install entire ecosystem
```

---

## Featured Libraries

### simple_kb - AI Knowledge Base

Searchable Eiffel knowledge base with AI-enhanced RAG:
- **4,613 classes** and **87,780 features** indexed
- **31 compiler error codes** with causes and fixes
- **14 design patterns** with Eiffel idioms
- **4-phase RAG cascade**: FAQ, FTS5, Query Expansion, LLM

```bash
kb search "void safety"
kb error VEVI
kb pattern singleton
kb ai "How do I handle attached types?"
```

### simple_gobo - SCOOP Parsing

GitHub Gobo (2024) with SCOOP inline separate support:

```eiffel
separate a_worker as l_worker do
    l_worker.do_work
end
```

### simple_rosetta - Algorithm Library

273 Rosetta Code solutions in Eiffel with contracts.

---

## Library Categories

### Data Formats
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_json](https://github.com/simple-eiffel/simple_json) | JSON with Schema, Patch, Pointer | Yes |
| [simple_csv](https://github.com/simple-eiffel/simple_csv) | RFC 4180 CSV parsing | Yes |
| [simple_xml](https://github.com/simple-eiffel/simple_xml) | XML parsing with XPath | Yes |
| [simple_yaml](https://github.com/simple-eiffel/simple_yaml) | YAML 1.2 parser | Yes |
| [simple_toml](https://github.com/simple-eiffel/simple_toml) | TOML configuration | |

### Web and Networking
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_http](https://github.com/simple-eiffel/simple_http) | HTTP client | Yes |
| [simple_web](https://github.com/simple-eiffel/simple_web) | Web framework | Yes |
| [simple_websocket](https://github.com/simple-eiffel/simple_websocket) | WebSocket client/server | |
| [simple_smtp](https://github.com/simple-eiffel/simple_smtp) | Email sending | Yes |
| [simple_grpc](https://github.com/simple-eiffel/simple_grpc) | gRPC protocol | |

### Security and Auth
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_jwt](https://github.com/simple-eiffel/simple_jwt) | JWT tokens | Yes |
| [simple_encryption](https://github.com/simple-eiffel/simple_encryption) | AES, RSA, hashing | Yes |

### Data and Storage
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_sql](https://github.com/simple-eiffel/simple_sql) | SQLite with fluent API | Yes |
| [simple_cache](https://github.com/simple-eiffel/simple_cache) | LRU cache + Redis | Yes |
| [simple_mq](https://github.com/simple-eiffel/simple_mq) | Message queues | Yes |

### AI and Knowledge
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_kb](https://github.com/simple-eiffel/simple_kb) | Knowledge base with RAG | Yes |
| [simple_ai_client](https://github.com/simple-eiffel/simple_ai_client) | OpenAI, Anthropic, Ollama | Yes |
| [simple_rosetta](https://github.com/simple-eiffel/simple_rosetta) | 273 algorithm implementations | |

### Infrastructure
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_docker](https://github.com/simple-eiffel/simple_docker) | Container management | Yes |
| [simple_k8s](https://github.com/simple-eiffel/simple_k8s) | Kubernetes orchestration | |
| [simple_scheduler](https://github.com/simple-eiffel/simple_scheduler) | Job scheduling, cron | |
| [simple_telemetry](https://github.com/simple-eiffel/simple_telemetry) | Tracing, metrics | |

### Developer Tools
| Library | Description |
|---------|-------------|
| [simple_lsp](https://github.com/simple-eiffel/simple_lsp) | VS Code language server |
| [simple_pkg](https://github.com/simple-eiffel/simple_pkg) | Package manager |
| [simple_notebook](https://github.com/simple-eiffel/simple_notebook) | Interactive Eiffel |
| [simple_testing](https://github.com/simple-eiffel/simple_testing) | Test framework |
| [simple_eiffel_parser](https://github.com/simple-eiffel/simple_eiffel_parser) | Eiffel source parser |
| [simple_gobo](https://github.com/simple-eiffel/simple_gobo) | GitHub Gobo 2024 |

### Utilities
| Library | Description |
|---------|-------------|
| [simple_uuid](https://github.com/simple-eiffel/simple_uuid) | UUID v4 generation |
| [simple_datetime](https://github.com/simple-eiffel/simple_datetime) | Date/time handling |
| [simple_regex](https://github.com/simple-eiffel/simple_regex) | Pattern matching |
| [simple_validation](https://github.com/simple-eiffel/simple_validation) | Input validation |
| [simple_template](https://github.com/simple-eiffel/simple_template) | Mustache templates |
| [simple_logger](https://github.com/simple-eiffel/simple_logger) | Structured logging |

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

*75+ libraries. One ecosystem. Modern Eiffel.*