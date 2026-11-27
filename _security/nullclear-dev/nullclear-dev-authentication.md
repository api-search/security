---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nullclear-dev-a2a-api-openapi.yml
  format: yaml
  label: NullClear A2A API
  slug: nullclear-dev-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-a2a-api-openapi.yml
- filename: nullclear-dev-bazaar-oracles-api-openapi.yml
  format: yaml
  label: NullClear Bazaar Oracles API
  slug: nullclear-dev-bazaar-oracles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-bazaar-oracles-api-openapi.yml
- filename: nullclear-dev-escrow-clearinghouse-api-openapi.yml
  format: yaml
  label: NullClear Escrow Clearinghouse API
  slug: nullclear-dev-escrow-clearinghouse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-escrow-clearinghouse-api-openapi.yml
- filename: nullclear-dev-firewall-pro-suite-api-openapi.yml
  format: yaml
  label: NullClear Firewall Pro Suite API
  slug: nullclear-dev-firewall-pro-suite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-firewall-pro-suite-api-openapi.yml
- filename: nullclear-dev-forensics-simulation-api-openapi.yml
  format: yaml
  label: NullClear Forensics & Simulation API
  slug: nullclear-dev-forensics-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-forensics-simulation-api-openapi.yml
- filename: nullclear-dev-reputation-kya-api-openapi.yml
  format: yaml
  label: NullClear Reputation & KYA API
  slug: nullclear-dev-reputation-kya-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-reputation-kya-api-openapi.yml
- filename: nullclear-dev-sandbox-api-openapi.yml
  format: yaml
  label: NullClear Sandbox API
  slug: nullclear-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-sandbox-api-openapi.yml
- filename: nullclear-dev-telemetry-api-openapi.yml
  format: yaml
  label: NullClear Telemetry API
  slug: nullclear-dev-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullclear-dev/openapi/nullclear-dev-telemetry-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NullClear Authentication
name_suffix: Authentication
oauth_flows: []
overview: NullClear secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NullClear
provider_slug: nullclear-dev
scheme_count: 2
schemes:
- description: x402 payment signature header containing EIP-3009 transfer authorization
  in: header
  name: x402
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/api-nullclear-dev-openapi.json
  - openapi/nullclear-dev-openapi.json
  type: apiKey
- description: Sign-In-With-X wallet identity header
  in: header
  name: siwx
  parameter: SIGN-IN-WITH-X
  sources:
  - openapi/api-nullclear-dev-openapi.json
  - openapi/nullclear-dev-openapi.json
  type: apiKey
slug: nullclear-dev-authentication
source_filename: nullclear-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/api-nullclear-dev-openapi.json, openapi/nullclear-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 payment signature header containing EIP-3009 transfer authorization\n  sources:\n  - openapi/api-nullclear-dev-openapi.json\n  - openapi/nullclear-dev-openapi.json\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: SIGN-IN-WITH-X\n  description: Sign-In-With-X wallet identity header\n  sources:\n  - openapi/api-nullclear-dev-openapi.json\n  - openapi/nullclear-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nullclear-dev/authentication/nullclear-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Blockchain
- Security
- LLM
---
