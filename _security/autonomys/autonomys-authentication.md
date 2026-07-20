---
api_key_in:
- header
api_specs:
- filename: autonomys-auto-drive-openapi.json
  format: json
  label: Autonomys Auto Drive API
  slug: autonomys-auto-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autonomys/refs/heads/main/openapi/autonomys-auto-drive-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Autonomys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autonomys secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Autonomys
provider_slug: autonomys
scheme_count: 2
schemes:
- description: 'Bearer token for authentication. Example: Bearer <token>. Could be either an API key or a JWT token.'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/autonomys-auto-drive-openapi.json
  type: apiKey
- description: 'Used for differentiating between different auth providers. For most use cases: X-Auth-Provider: apikey'
  in: header
  name: provider
  parameter: X-Auth-Provider
  sources:
  - openapi/autonomys-auto-drive-openapi.json
  type: apiKey
slug: autonomys-authentication
source_filename: autonomys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/autonomys-auto-drive-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Bearer token for authentication. Example: Bearer <token>. Could be either an\n    API key or a JWT token.'\n  sources:\n  - openapi/autonomys-auto-drive-openapi.json\n- name: provider\n  type: apiKey\n  in: header\n  parameter: X-Auth-Provider\n  description: 'Used for differentiating between different auth providers. For most use cases:\n    X-Auth-Provider: apikey'\n  sources:\n  - openapi/autonomys-auto-drive-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonomys/refs/heads/main/authentication/autonomys-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Crypto
- Blockchain
- Web3
- Decentralized Storage
- Storage
- AI Agents
- IPFS
- TypeScript SDK
---
