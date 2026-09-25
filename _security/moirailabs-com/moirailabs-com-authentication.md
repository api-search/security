---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moirailabs-com-openapi.yml
  format: yaml
  label: Moirai Labs API
  slug: moirai-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/openapi/moirailabs-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Moirailabs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moirai Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moirai Labs
provider_slug: moirailabs-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moirailabs-com-openapi.yml
  type: http
slug: moirailabs-com-authentication
source_filename: moirailabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/moirailabs-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/moirailabs-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moirailabs-com/refs/heads/main/authentication/moirailabs-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Blockchain
- Smart Contracts
- Web3
- Analytics
- cohort-analysis
- Wallet Profiling
- Ethereum
- AI Agents
- A2A
- MCP
- Agent-Native
---
