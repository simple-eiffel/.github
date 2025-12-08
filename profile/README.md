
  ## Getting Started

  Install the entire ecosystem with **simple_setup**:

  ```bash
  git clone https://github.com/simple-eiffel/simple_setup.git
  cd simple_setup
  simple_setup install --all

  Or install individual libraries:

  simple_setup install simple_json simple_csv simple_process

  ---
  Library Layers

  | Layer      | Purpose        | Key Libraries                                                       |
  |------------|----------------|---------------------------------------------------------------------|
  | Foundation | Core utilities | simple_json, simple_csv, simple_hash, simple_uuid, simple_regex     |
  | Platform   | OS integration | simple_env, simple_console, simple_registry, simple_win32_api       |
  | Service    | Business logic | simple_sql, simple_smtp, simple_jwt, simple_http, simple_encryption |
  | API        | Facades        | simple_foundation_api, simple_service_api, simple_web               |

  ---
  Featured Libraries

  | Library                                       | Description                                     |
  |-----------------------------------------------|-------------------------------------------------|
  | https://github.com/simple-eiffel/simple_json  | JSON parsing, Schema validation, Pointer, Patch |
  | https://github.com/simple-eiffel/simple_sql   | SQLite with fluent API                          |
  | https://github.com/simple-eiffel/simple_web   | HTTP server framework                           |
  | https://github.com/simple-eiffel/simple_jwt   | JSON Web Token handling                         |
  | https://github.com/simple-eiffel/simple_setup | Package manager & installer                     |

  ---
  Design Principles

  - Design by Contract - Preconditions, postconditions, invariants
  - Void Safety - Compile-time null protection
  - SCOOP Ready - Concurrency support
  - 100% Test Coverage - Comprehensive test suites
  - AI-Assisted Development - Built with Claude

  ---
  Resources

  - https://www.eiffel.org/downloads
  - https://www.eiffel.org/doc/
  - https://ecma-international.org/publications-and-standards/standards/ecma-367/

  ---
  Create the .github repo, then add this as profile/README.md.

