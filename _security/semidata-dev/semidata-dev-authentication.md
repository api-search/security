---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: semidata-dev-agent-integration-api-openapi.yml
  format: yaml
  label: semidata-dev Agent Integration API
  slug: semidata-dev-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/semidata-dev/openapi/semidata-dev-agent-integration-api-openapi.yml
- filename: semidata-dev-supply-chain-intelligence-api-openapi.yml
  format: yaml
  label: semidata-dev Supply Chain Intelligence API
  slug: semidata-dev-supply-chain-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/semidata-dev/openapi/semidata-dev-supply-chain-intelligence-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Semidata Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: semidata-dev secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: semidata-dev
provider_slug: semidata-dev
scheme_count: 2
schemes:
- description: 'Free tier: 100 req/day. Request at semidata.dev'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/semidata-dev-openapi.yml
  type: apiKey
- description: x402 micropayment  -  $0.005 USDC on Base mainnet. No signup.
  in: header
  name: X402Payment
  parameter: X-Payment
  sources:
  - openapi/semidata-dev-openapi.yml
  type: apiKey
slug: semidata-dev-authentication
source_filename: semidata-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/semidata-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Free tier: 100 req/day. Request at semidata.dev'\n  sources:\n  - openapi/semidata-dev-openapi.yml\n- name: X402Payment\n  type: apiKey\n  in: header\n  parameter: X-Payment\n  description: x402 micropayment  -  $0.005 USDC on Base mainnet. No signup.\n  sources:\n  - openapi/semidata-dev-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/semidata-dev/authentication/semidata-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Semiconductor
- Quantum
- SupplyChain
- DataAPI
- Intelligence
---
