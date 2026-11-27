---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: EDGE Authentication
name_suffix: Authentication
oauth_flows: []
overview: EDGE secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EDGE
provider_slug: agent-z-app
scheme_count: 2
schemes:
- description: edge_live_... member key
  name: memberKey
  scheme: bearer
  sources:
  - openapi/agent-z-app-openapi.json
  type: http
- description: Base transaction hash paying 0.25 USDC to the payTo address. Single use.
  in: header
  name: paymentTx
  parameter: X-Payment-Tx
  sources:
  - openapi/agent-z-app-openapi.json
  type: apiKey
slug: agent-z-app-authentication
source_filename: agent-z-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/agent-z-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: memberKey\n  type: http\n  scheme: bearer\n  description: edge_live_... member key\n  sources:\n  - openapi/agent-z-app-openapi.json\n- name: paymentTx\n  type: apiKey\n  in: header\n  parameter: X-Payment-Tx\n  description: Base transaction hash paying 0.25 USDC to the payTo address. Single use.\n  sources:\n  - openapi/agent-z-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agent-z-app/authentication/agent-z-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Finance
- Cryptocurrency
- Trading
- Automation
- Tokenization
---
