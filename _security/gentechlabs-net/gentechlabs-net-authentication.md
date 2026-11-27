---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gentechlabs-net-gentech-labs-x402-gateway-api-openapi.yml
  format: yaml
  label: GenTech Labs GenTech Labs X402 Gateway API
  slug: gentechlabs-net-gentech-labs-x402-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-gentech-labs-x402-gateway-api-openapi.yml
- filename: gentechlabs-net-health-api-openapi.yml
  format: yaml
  label: GenTech Labs Health API
  slug: gentechlabs-net-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-health-api-openapi.yml
- filename: gentechlabs-net-openapi-json-api-openapi.yml
  format: yaml
  label: GenTech Labs Openapi.json API
  slug: gentechlabs-net-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-openapi-json-api-openapi.yml
- filename: gentechlabs-net-paid-api-openapi.yml
  format: yaml
  label: GenTech Labs Paid API
  slug: gentechlabs-net-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-paid-api-openapi.yml
- filename: gentechlabs-net-status-api-openapi.yml
  format: yaml
  label: GenTech Labs Status API
  slug: gentechlabs-net-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-status-api-openapi.yml
- filename: gentechlabs-net-well-known-api-openapi.yml
  format: yaml
  label: GenTech Labs .well Known API
  slug: gentechlabs-net-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gentechlabs-net/openapi/gentechlabs-net-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GenTech Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: GenTech Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GenTech Labs
provider_slug: gentechlabs-net
scheme_count: 1
schemes:
- description: 'x402 payment proof. Call without a proof to receive HTTP 402 with payment requirements (USD₮0 / USD Coin, payable on 5 settlement rails: xlayer, base, avalanche, algorand, solana). Pay per rail and retry with the x402 authorization header.'
  name: x402
  scheme: bearer
  sources:
  - openapi/gentechlabs-net-openapi.yml
  type: http
slug: gentechlabs-net-authentication
source_filename: gentechlabs-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gentechlabs-net-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: x402\n  type: http\n  scheme: bearer\n  description: 'x402 payment proof. Call without a proof to receive HTTP 402 with payment requirements\n    (USD₮0 / USD Coin, payable on 5 settlement rails: xlayer, base, avalanche, algorand, solana).\n    Pay per rail and retry with the x402 authorization header.'\n  sources:\n  - openapi/gentechlabs-net-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gentechlabs-net/authentication/gentechlabs-net-authentication.yml
summary_line: http · 1 scheme
tags:
- AgentEconomy
- Blockchain
- Payments
- USDC
- Identity
---
