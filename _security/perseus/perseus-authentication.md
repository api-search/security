---
api_key_in: []
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Perseus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perseus secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perseus
provider_slug: perseus
scheme_count: 1
schemes:
- device_flow: true
  name: cli-token
  sources:
  - https://perseus.computer/docs
  type: token
  via: perseus login
slug: perseus-authentication
source_filename: perseus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://perseus.computer/docs\ndocs: https://perseus.computer/docs\nsummary:\n  types: [token]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Authentication is handled through the Perseus CLI, not a public HTTP API. `perseus login`\n    performs an interactive browser-based sign-in; `perseus login --device` runs a device\n    authorization flow for headless/remote environments. The resulting token is stored by the CLI\n    and used for subsequent commands. No API-key header or documented OAuth2 authorization-server\n    endpoints are published as of this pass (no OpenAPI, no /.well-known/openid-configuration or\n    /oauth-authorization-server — both returned 404).\nschemes:\n- name: cli-token\n  type: token\n  via: perseus login\n  device_flow: true\n  sources: [https://perseus.computer/docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perseus/refs/heads/main/authentication/perseus-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Artificial Intelligence
- Developer Tools
- Code Search
- Semantic Search
- Coding Agents
- AI Agents
- Latent Space
- CLI
- Agent Skills
- Y Combinator
---
