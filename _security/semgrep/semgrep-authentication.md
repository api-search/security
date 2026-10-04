---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Semgrep Guardian supports two authentication methods: OAuth for Claude Code and API token for other coding agents.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Semgrep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semgrep declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Semgrep
provider_slug: semgrep
scheme_count: 2
schemes:
- evidence: Claude Code uses Semgrep's hosted remote server and authenticates through OAuth, so developers don't need to install or run the Semgrep CLI.
  name: OAuth
  type: oauth2
- evidence: Each developer signs in with `semgrep login`, which opens a browser-based login flow.
  name: API token
  type: apiKey
slug: semgrep-authentication
source_filename: semgrep-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.semgrep.dev/semgrep-guardian/authentication.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.semgrep.dev/semgrep-guardian/authentication.md\nsources:\n- https://docs.semgrep.dev/semgrep-guardian/authentication.md\n- https://docs.semgrep.dev/semgrep-guardian/quickstart.md\n- https://docs.semgrep.dev/semgrep-guardian/choose-your-setup.md\n- https://docs.semgrep.dev/semgrep-guardian/ide-setup/claude-code.md\ndescription: 'Semgrep Guardian supports two authentication methods: OAuth for Claude Code and API token for other coding agents.'\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Claude Code uses Semgrep's hosted remote server and authenticates through OAuth, so developers don't need to install or run the Semgrep\n    CLI.\n- type: apiKey\n  name: API token\n  evidence: Each developer signs in with `semgrep login`, which opens a browser-based login flow.\ndocs: https://docs.semgrep.dev/semgrep-guardian/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semgrep/refs/heads/main/authentication/semgrep-authentication.yml
summary_line: 2 schemes
tags:
- Static Analysis
- SAST
- Application Security
- Supply Chain
- Secrets Detection
- Developer Tools
- DevSecOps
---
