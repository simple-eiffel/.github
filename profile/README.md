<p align="center">
  <img src="https://raw.githubusercontent.com/simple-eiffel/claude_eiffel_op_docs/main/artwork/LOGO.png" alt="Simple Eiffel" width="300">
</p>

# Simple Eiffel

**71 production-ready Eiffel libraries for modern software development**

[![Libraries](https://img.shields.io/badge/libraries-71-blue)](https://github.com/simple-eiffel)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Eiffel](https://img.shields.io/badge/Eiffel-25.02-orange)](https://www.eiffel.org/)

---

## What's New

- **QUICK APIs** - 17 libraries now have zero-configuration beginner facades
- **simple_pkg** - Package manager for the ecosystem
- **simple_lsp** - VS Code language server with DbC Heatmap visualization
- **simple_docker** - Container management from Eiffel
- **TOON format** - Token-optimized notation reducing LLM costs 30-60%

---

## Quick Start

### Windows

1. Install [EiffelStudio 25.02](https://www.eiffel.org/downloads)
2. Set environment variable:
   ```cmd
   setx SIMPLE_EIFFEL D:\path\to\simple_eiffel
   ```
3. Add to your ECF:
   ```xml
   <library name="simple_json" location="$SIMPLE_EIFFEL/simple_json/simple_json.ecf"/>
   ```

### Linux / WSL2

1. Download and extract EiffelStudio:
   ```bash
   wget https://ftp.eiffel.com/pub/download/25.02/Eiffel_25.02_rev_98732-linux-x86-64.tar.bz2
   tar xjf Eiffel_25.02_rev_98732-linux-x86-64.tar.bz2
   mv Eiffel_25.02 ~/simple_eiffel/
   ```

2. Add to `~/.bashrc`:
   ```bash
   # Simple Eiffel ecosystem
   export SIMPLE_EIFFEL=$HOME/simple_eiffel

   # EiffelStudio
   export ISE_EIFFEL=$HOME/simple_eiffel/Eiffel_25.02
   export ISE_PLATFORM=linux-x86-64
   export ISE_LIBRARY=$ISE_EIFFEL
   export PATH=$ISE_EIFFEL/studio/spec/$ISE_PLATFORM/bin:$PATH
   ```

3. Compile and test:
   ```bash
   cd $SIMPLE_EIFFEL/simple_json
   ec -batch -config simple_json.ecf -target simple_json_tests -c_compile
   ./EIFGENs/simple_json_tests/W_code/simple_json
   # Result: 214 passed, 0 failed
   ```

### Package Manager

Use [simple_pkg](https://github.com/simple-eiffel/simple_pkg) to install libraries:
```bash
simple_pkg install simple_json
simple_pkg install all     # Install entire ecosystem
```

---

## Beginner-Friendly QUICK APIs

Every QUICK class provides one-liner operations with sensible defaults:

```eiffel
-- JSON
create json.make
name := json.get_string (data, "$.users[0].name")

-- Validation
create v.make
if v.email ("user@example.com") then ...

-- Caching with "remember" pattern
create cache.make
value := cache.remember ("key", agent compute_expensive_value)

-- Regex with built-in validators
create rx.make
if rx.is_email (input) and rx.is_url (link) then ...

-- YAML config files
create yaml.make
host := yaml.get_string (config, "database.host")
```

**Libraries with QUICK APIs:** json, cache, validation, template, csv, xml, yaml, regex, sql, http, smtp, jwt, encryption, mq, ai_client, web, docker

---

## Library Categories

### Data Formats
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_json](https://github.com/simple-eiffel/simple_json) | JSON with Schema validation, Patch, Pointer | Yes |
| [simple_csv](https://github.com/simple-eiffel/simple_csv) | RFC 4180 CSV parsing | Yes |
| [simple_xml](https://github.com/simple-eiffel/simple_xml) | XML parsing with XPath | Yes |
| [simple_yaml](https://github.com/simple-eiffel/simple_yaml) | YAML 1.2 parser | Yes |
| [simple_toml](https://github.com/simple-eiffel/simple_toml) | TOML configuration | |
| [simple_markdown](https://github.com/simple-eiffel/simple_markdown) | Markdown to HTML | |
| [simple_toon](https://github.com/simple-eiffel/simple_toon) | Token-optimized notation for LLMs | |

### Web & Networking
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_http](https://github.com/simple-eiffel/simple_http) | HTTP client | Yes |
| [simple_web](https://github.com/simple-eiffel/simple_web) | Web framework | Yes |
| [simple_websocket](https://github.com/simple-eiffel/simple_websocket) | WebSocket client/server | |
| [simple_smtp](https://github.com/simple-eiffel/simple_smtp) | Email sending | Yes |
| [simple_grpc](https://github.com/simple-eiffel/simple_grpc) | gRPC protocol | |
| [simple_cors](https://github.com/simple-eiffel/simple_cors) | CORS middleware | |
| [simple_htmx](https://github.com/simple-eiffel/simple_htmx) | HTMX integration | |
| [simple_alpine](https://github.com/simple-eiffel/simple_alpine) | Alpine.js integration | |

### Security & Auth
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_jwt](https://github.com/simple-eiffel/simple_jwt) | JWT tokens | Yes |
| [simple_encryption](https://github.com/simple-eiffel/simple_encryption) | AES, RSA, hashing | Yes |
| [simple_hash](https://github.com/simple-eiffel/simple_hash) | SHA, MD5, HMAC | |

### Data & Storage
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_sql](https://github.com/simple-eiffel/simple_sql) | SQLite with fluent API | Yes |
| [simple_cache](https://github.com/simple-eiffel/simple_cache) | LRU cache + Redis | Yes |
| [simple_mq](https://github.com/simple-eiffel/simple_mq) | Message queues | Yes |
| [simple_oracle](https://github.com/simple-eiffel/simple_oracle) | Context persistence | |

### Infrastructure
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_docker](https://github.com/simple-eiffel/simple_docker) | Container management | Yes |
| [simple_process](https://github.com/simple-eiffel/simple_process) | Process spawning | |
| [simple_scheduler](https://github.com/simple-eiffel/simple_scheduler) | Job scheduling, cron | |
| [simple_telemetry](https://github.com/simple-eiffel/simple_telemetry) | Tracing, metrics | |
| [simple_ipc](https://github.com/simple-eiffel/simple_ipc) | Inter-process communication | |

### AI & Machine Learning
| Library | Description | QUICK |
|---------|-------------|:-----:|
| [simple_ai_client](https://github.com/simple-eiffel/simple_ai_client) | OpenAI, Anthropic, Ollama | Yes |

### Utilities
| Library | Description |
|---------|-------------|
| [simple_uuid](https://github.com/simple-eiffel/simple_uuid) | UUID v4 generation |
| [simple_base64](https://github.com/simple-eiffel/simple_base64) | Base64 encoding |
| [simple_datetime](https://github.com/simple-eiffel/simple_datetime) | Date/time handling |
| [simple_decimal](https://github.com/simple-eiffel/simple_decimal) | Arbitrary precision |
| [simple_fraction](https://github.com/simple-eiffel/simple_fraction) | Rational numbers |
| [simple_regex](https://github.com/simple-eiffel/simple_regex) | Pattern matching |
| [simple_validation](https://github.com/simple-eiffel/simple_validation) | Input validation |
| [simple_template](https://github.com/simple-eiffel/simple_template) | Mustache templates |
| [simple_logger](https://github.com/simple-eiffel/simple_logger) | Structured logging |
| [simple_i18n](https://github.com/simple-eiffel/simple_i18n) | Internationalization |
| [simple_cli](https://github.com/simple-eiffel/simple_cli) | CLI argument parsing |
| [simple_config](https://github.com/simple-eiffel/simple_config) | Configuration management |
| [simple_rate_limiter](https://github.com/simple-eiffel/simple_rate_limiter) | Rate limiting |

### Platform & System
| Library | Description |
|---------|-------------|
| [simple_env](https://github.com/simple-eiffel/simple_env) | Environment variables |
| [simple_file](https://github.com/simple-eiffel/simple_file) | File operations |
| [simple_console](https://github.com/simple-eiffel/simple_console) | Terminal I/O |
| [simple_clipboard](https://github.com/simple-eiffel/simple_clipboard) | Clipboard access |
| [simple_registry](https://github.com/simple-eiffel/simple_registry) | Windows registry |
| [simple_win32_api](https://github.com/simple-eiffel/simple_win32_api) | Win32 bindings |
| [simple_platform_api](https://github.com/simple-eiffel/simple_platform_api) | Cross-platform facade |

### Developer Tools
| Library | Description |
|---------|-------------|
| [simple_lsp](https://github.com/simple-eiffel/simple_lsp) | VS Code language server |
| [simple_pkg](https://github.com/simple-eiffel/simple_pkg) | Package manager |
| [simple_testing](https://github.com/simple-eiffel/simple_testing) | Test framework |
| [simple_eiffel_parser](https://github.com/simple-eiffel/simple_eiffel_parser) | Eiffel source parser |
| [simple_ucf](https://github.com/simple-eiffel/simple_ucf) | Universe Configuration |

### API Facades
| Library | Description |
|---------|-------------|
| [simple_foundation_api](https://github.com/simple-eiffel/simple_foundation_api) | Core utilities bundle |
| [simple_service_api](https://github.com/simple-eiffel/simple_service_api) | Services bundle |
| [simple_app_api](https://github.com/simple-eiffel/simple_app_api) | Full stack bundle |

---

## VS Code Integration

Install **Simple Eiffel LSP** from the VS Code marketplace:
- Syntax highlighting
- Go to definition
- **DbC Heatmap** - Visualize contract coverage across your codebase

---

## Cross-Platform Support

| Platform | Status | Libraries | Notes |
|----------|--------|-----------|-------|
| **Windows** | ✅ Full | 71/71 | Primary development platform |
| **Linux** | ✅ Tested | 60+/71 | Platform-agnostic libraries verified |
| **WSL2** | ✅ Tested | 60+/71 | [Setup guide](https://github.com/simple-eiffel/claude_eiffel_op_docs/blob/main/deployment/WSL2_LINUX_SETUP.md) |
| **macOS** | 🔄 Untested | 60+/71 | EiffelStudio available |

### Linux Compatibility Roadmap

| Library | Current Status | Linux Solution | Effort |
|---------|----------------|----------------|--------|
| simple_docker | ✅ Done | Unix socket `/var/run/docker.sock` | Done |
| simple_ipc | ✅ Done | Unix domain sockets implemented | Done |
| simple_pkg | ✅ Done | ~/.bashrc env var support | Done |
| simple_oracle | ✅ Done | Documentation updated | Done |
| simple_lsp | Needs work | Path abstraction | Easy |
| simple_process | Win32 API | POSIX fork/exec | Medium |
| simple_mmap | Win32 API | POSIX mmap() | Medium |
| simple_clipboard | Win32 API | xclip/wl-copy | Medium |
| simple_console | Win32 API | ANSI escapes | Medium |
| simple_gui_designer | WEL | Windows only | N/A |
| simple_win32_api | By design | Windows only | N/A |
| simple_registry | By design | Windows only | N/A |

### Linux Notes
- Remove `EIFGENs/` directory before compiling (clears Windows artifacts)
- Set `ISE_LIBRARY=$ISE_EIFFEL` (not `$ISE_EIFFEL/library`)
- All ECF files use forward slashes for `$SIMPLE_EIFFEL` paths

---

## Design Principles

- **Design by Contract** - Preconditions, postconditions, invariants on every feature
- **Void Safety** - Compile-time null protection
- **SCOOP Compatible** - All libraries work with Eiffel's concurrency model
- **Human+AI Development** - Built collaboratively with Claude (Anthropic)

---

## Documentation

- **Website**: [simple-eiffel.github.io](https://simple-eiffel.github.io)
- **Each library**: `https://simple-eiffel.github.io/{library}/`

---

## Contributing

Issues and pull requests welcome. All code follows Eiffel's Design by Contract principles.

---

*71 libraries. One ecosystem. Modern Eiffel.*
