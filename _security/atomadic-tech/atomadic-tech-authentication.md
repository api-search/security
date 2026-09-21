---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: atomadic-tech-openapi.yml
  format: yaml
  label: AAAA Nexus API
  slug: aaaa-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomadic-tech/refs/heads/main/openapi/atomadic-tech-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Atomadic Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atomadic Tech secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Atomadic Tech
provider_slug: atomadic-tech
scheme_count: 3
schemes:
- description: API key obtained from https://atomadic.tech/pay
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/atomadic-tech-openapi.yml
  type: apiKey
- description: Base64-encoded USDC payment proof for x402 autonomous payment flow (Base L2, Polygon, or Solana)
  in: header
  name: X402PaymentProof
  parameter: X-Payment-Proof
  sources:
  - openapi/atomadic-tech-openapi.yml
  type: apiKey
- description: Admin token for privileged operations
  in: header
  name: AdminTokenAuth
  parameter: X-Admin-Token
  sources:
  - openapi/atomadic-tech-openapi.yml
  type: apiKey
slug: atomadic-tech-authentication
source_filename: atomadic-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/atomadic-tech-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key obtained from https://atomadic.tech/pay\n  sources:\n  - openapi/atomadic-tech-openapi.yml\n- name: X402PaymentProof\n  type: apiKey\n  in: header\n  parameter: X-Payment-Proof\n  description: Base64-encoded USDC payment proof for x402 autonomous payment flow (Base L2,\n    Polygon, or Solana)\n  sources:\n  - openapi/atomadic-tech-openapi.yml\n- name: AdminTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Admin-Token\n  description: Admin token for privileged operations\n  sources:\n  - openapi/atomadic-tech-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomadic-tech/refs/heads/main/authentication/atomadic-tech-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- AI Agents
- Agent Infrastructure
- MCP
- A2A
- x402
- Payments
- Compliance
- Security
- Trust
- Identity
- Escrow
- Inference
- Cryptography
---
