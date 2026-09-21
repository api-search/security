---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: taskhawktech-com-openapi.yml
  format: yaml
  label: Kevros Governance API
  slug: kevros-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/openapi/taskhawktech-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Taskhawktech Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaskHawk Systems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TaskHawk Systems
provider_slug: taskhawktech-com
scheme_count: 1
schemes:
- description: Get a trial key via POST /signup. 1,000-call trial allowance.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/taskhawktech-com-openapi.yml
  type: apiKey
slug: taskhawktech-com-authentication
source_filename: taskhawktech-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/taskhawktech-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Get a trial key via POST /signup. 1,000-call trial allowance.\n  sources:\n  - openapi/taskhawktech-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/authentication/taskhawktech-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Governance
- Agent Security
- Runtime Enforcement
- Policy Enforcement
- Provenance
- Compliance
- Prompt Injection Detection
- Media Attestation
- Post-Quantum Cryptography
- Formal Verification
- x402
- L402
- Machine Payments
- MCP
- A2A
- agent-native
- Government
- Defense
---
