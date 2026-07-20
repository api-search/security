---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Arga Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arga Labs secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arga Labs
provider_slug: arga-labs
scheme_count: 2
schemes:
- header: 'Authorization: Bearer <token>'
  name: apiKeyBearer
  prefix: arga_sk_
  provisioning:
  - Settings -> API Keys in the web app
  - arga login (device-scoped key stored at ~/.config/arga/config.json)
  quickstart_key:
    note: Email get-started signup yields a quickstart API key limited to 5 twin provisions.
  scheme: bearer
  token_type: API key
  type: http
  usage: Server-to-server calls — SDKs, CI jobs, scripts, local tools.
- name: jwtSession
  scheme: bearer
  token_type: JWT
  type: http
  usage: Web app sessions and user-scoped browser flows. Some GitHub configuration endpoints require a user session.
slug: arga-labs-authentication
source_filename: arga-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.argalabs.com/api-reference/auth\ndocs: https://docs.argalabs.com/api-reference/auth\nbase_url: https://api.argalabs.com\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_kinds:\n  - api_key\n  - jwt\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  token_type: API key\n  prefix: arga_sk_\n  usage: Server-to-server calls — SDKs, CI jobs, scripts, local tools.\n  header: 'Authorization: Bearer <token>'\n  provisioning:\n  - Settings -> API Keys in the web app\n  - arga login (device-scoped key stored at ~/.config/arga/config.json)\n  quickstart_key:\n    note: Email get-started signup yields a quickstart API key limited to 5 twin provisions.\n- name: jwtSession\n  type: http\n  scheme: bearer\n  token_type: JWT\n  usage: Web app sessions and user-scoped browser flows. Some GitHub configuration endpoints require a user session.\nnotes:\n- One account per email address; identity endpoints\
  \ return 409 when violated.\n- CLI/SDK/MCP all target https://api.argalabs.com by default; override with --api-url or ARGA_API_URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arga-labs/refs/heads/main/authentication/arga-labs-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- API Testing
- Sandboxes
- Digital Twins
- AI Agents
- Developer Tools
- Testing Infrastructure
- CI/CD
- Browser Testing
- MCP
- Mock Services
---
