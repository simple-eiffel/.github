
  # Simple Eiffel

  **Modern Eiffel libraries for practical software development**

  ---

  ## Getting Started

  Install the entire ecosystem with **simple_setup**:

  ```bash
  git clone https://github.com/simple-eiffel/simple_setup.git
  cd simple_setup
  simple_setup install --all```

  Or install individual libraries:

  simple_setup install simple_json simple_csv simple_process

  ---

  Library Layers

  | Layer      | Purpose        | Key Libraries                                         |
  |------------|----------------|-------------------------------------------------------|
  | Foundation | Core utilities | simple_json, simple_csv, simple_hash, simple_uuid     |
  | Platform   | OS integration | simple_env, simple_console, simple_registry           |
  | Service    | Business logic | simple_sql, simple_smtp, simple_jwt, simple_http      |
  | API        | Facades        | simple_foundation_api, simple_service_api, simple_web |

  ---

  Featured Libraries

  | Library                                       | Description                        |
  |-----------------------------------------------|------------------------------------|
  | https://github.com/simple-eiffel/simple_json  | JSON parsing and Schema validation |
  | https://github.com/simple-eiffel/simple_sql   | SQLite with fluent API             |
  | https://github.com/simple-eiffel/simple_web   | HTTP server framework              |
  | https://github.com/simple-eiffel/simple_setup | Package manager and installer      |

  ---

  Design Principles

  - Design by Contract - Preconditions, postconditions, invariants
  - Void Safety - Compile-time null protection
  - SCOOP Ready - Concurrency support
  - AI-Assisted Development - Built with Claude

