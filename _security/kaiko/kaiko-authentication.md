---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kaiko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaiko secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kaiko
provider_slug: kaiko
scheme_count: 1
schemes:
- description: Kaiko client API key delivered in the X-Api-Key header.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/kaiko-openapi.yml
  type: apiKey
slug: kaiko-authentication
source_filename: kaiko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kaiko-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Kaiko client API key delivered in the X-Api-Key header.\n  sources:\n  - openapi/kaiko-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaiko/refs/heads/main/authentication/kaiko-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- Market Data
- Institutional
- FX
- Indices
- On-Chain
- Streaming
---
