---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nebula Security Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: Nebula Security secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: Nebula Security
provider_slug: nebula-security
scheme_count: 2
schemes:
- cli_flag: --api-key
  env: VEGA_API_KEY
  key_prefix: vega_
  name: VegaApiKey
  note: Highest-precedence credential; suitable for headless/CI use.
  precedence: 1
  type: apiKey
- cli: vega auth login
  flow: browser-login
  headless_flag: --headless
  name: VegaOAuthLogin
  note: Stored OAuth token from an interactive browser login; used when VEGA_API_KEY is unset.
  precedence: 2
  type: oauth2
slug: nebula-security-authentication
source_filename: nebula-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/NebuSec/vega-skill/blob/main/skills/vega-cli/SKILL.md\nnote: >-\n  No public OpenAPI is published, so this profile is derived from the Vega CLI\n  authentication documentation rather than a machine-readable securityScheme.\n  The Vega backend (VEGA_API_URL, default production) authenticates with either a\n  bearer API key or an OAuth browser login.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_prefix: vega_\n  oauth2_flows: [browser-login]\nschemes:\n- name: VegaApiKey\n  type: apiKey\n  key_prefix: vega_\n  env: VEGA_API_KEY\n  cli_flag: --api-key\n  precedence: 1\n  note: Highest-precedence credential; suitable for headless/CI use.\n- name: VegaOAuthLogin\n  type: oauth2\n  flow: browser-login\n  cli: vega auth login\n  headless_flag: --headless\n  precedence: 2\n  note: Stored OAuth token from an interactive browser login; used when VEGA_API_KEY is unset.\nverify: vega auth status\
  \ --json\nunauthenticated_exit_code: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nebula-security/refs/heads/main/authentication/nebula-security-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Application Security
- Code Scanning
- Artificial Intelligence
- Developer Tools
- CLI
---
