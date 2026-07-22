---
api_key_in:
- header
api_specs:
- filename: m-0-orchestration-openapi.json
  format: json
  label: M0 Orchestration API
  slug: m0-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/m-0/refs/heads/main/openapi/m-0-orchestration-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: M 0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: M 0 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: M 0
provider_slug: m-0
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/m-0-orchestration-openapi.json
  type: apiKey
slug: m-0-authentication
source_filename: m-0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/m-0-orchestration-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/m-0-orchestration-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-0/refs/heads/main/authentication/m-0-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Stablecoin
- Cryptocurrency
- Blockchain
- Payments
- DeFi
- Web3
- Cross-Chain
- Tokenization
- Infrastructure
---
