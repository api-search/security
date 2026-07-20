---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Iyk Authentication
name_suffix: Authentication
oauth_flows: []
overview: IYK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IYK
provider_slug: iyk
scheme_count: 1
schemes:
- description: Team-scoped API key. Required on all Core, Modules, and Self-Service endpoints except the public GET /chips/find validation endpoint.
  in: header
  name: iykApiKey
  parameter: x-iyk-api-key
  sources:
  - https://docs.iyk.app/api-core/chips
  type: apiKey
slug: iyk-authentication
source_filename: iyk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.iyk.app/api-overview\ndocs: https://docs.iyk.app/api-quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    IYK authenticates API requests with a team-scoped API key passed in the\n    x-iyk-api-key request header. The public tap-resolution endpoint\n    GET /chips/find does not require the key. Keys are issued per team from\n    the IYK Studio dashboard.\nschemes:\n- name: iykApiKey\n  type: apiKey\n  in: header\n  parameter: x-iyk-api-key\n  description: >-\n    Team-scoped API key. Required on all Core, Modules, and Self-Service\n    endpoints except the public GET /chips/find validation endpoint.\n  sources: [https://docs.iyk.app/api-core/chips]\npublic_endpoints:\n- method: GET\n  path: /chips/find\n  note: Public tap validation from URL parameters; no API key required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iyk/refs/heads/main/authentication/iyk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- NFC
- Phygital
- Blockchain
- NFT
- POAP
- Chips
- Authentication
- Fan Engagement
- Web3
---
