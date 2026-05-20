# AGENTS.md

## Cursor Cloud specific instructions

### Repository Overview

This is a **data-only repository** containing a single Czech (Čeština) translation file (`cs.json`) for [Apache Guacamole Client](https://github.com/apache/guacamole-client). There is no application code, build system, package manager, or test framework.

### Development Workflow

- **Lint/Validate**: Use `python3 -c "import json; json.load(open('cs.json'))"` or `jq empty cs.json` to validate the JSON.
- **Build**: N/A — no build step exists.
- **Tests**: N/A — no automated test suite exists. Validation is JSON syntax checking.
- **Run**: N/A — this is a static translation resource, not a runnable application.

### Key Notes

- The file `cs.json` must always be valid JSON (UTF-8 encoded).
- Translation keys must match the structure of the upstream English source at `guacamole/src/main/frontend/src/translations/en.json` in the [apache/guacamole-client](https://github.com/apache/guacamole-client) repo.
- Both `python3` and `jq` are available in the environment for JSON validation.
- No dependencies need to be installed — the environment is ready to use out of the box.
