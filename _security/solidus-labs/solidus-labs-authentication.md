---
api_key_in:
- query
api_specs:
- filename: solidus-labs-address-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Address API API
  slug: solidus-labs-address-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-address-api-api-openapi.yml
- filename: solidus-labs-chain-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Chain API API
  slug: solidus-labs-chain-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-chain-api-api-openapi.yml
- filename: solidus-labs-corrections-api-openapi.yml
  format: yaml
  label: Solidus Labs Corrections API
  slug: solidus-labs-corrections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-corrections-api-openapi.yml
- filename: solidus-labs-latest-api-openapi.yml
  format: yaml
  label: Solidus Labs Latest API
  slug: solidus-labs-latest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-latest-api-openapi.yml
- filename: solidus-labs-scams-api-openapi.yml
  format: yaml
  label: Solidus Labs Scams API
  slug: solidus-labs-scams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-scams-api-openapi.yml
- filename: solidus-labs-token-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Token API API
  slug: solidus-labs-token-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-token-api-api-openapi.yml
- filename: solidus-labs-webhooks-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Webhooks API API
  slug: solidus-labs-webhooks-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-webhooks-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Solidus Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solidus Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Solidus Labs
provider_slug: solidus-labs
scheme_count: 1
schemes:
- in: query
  name: sec0
  parameter: apikey
  sources:
  - openapi/solidus-labs-tokensniffer-addresses-openapi.yml
  - openapi/solidus-labs-tokensniffer-pairs-openapi.yml
  - openapi/solidus-labs-tokensniffer-tokens-openapi.yml
  - openapi/solidus-labs-tokensniffer-webhooks-openapi.yml
  type: apiKey
slug: solidus-labs-authentication
source_filename: solidus-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/solidus-labs-tokensniffer-addresses-openapi.yml, openapi/solidus-labs-tokensniffer-pairs-openapi.yml,\n  openapi/solidus-labs-tokensniffer-tokens-openapi.yml, openapi/solidus-labs-tokensniffer-webhooks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: sec0\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/solidus-labs-tokensniffer-addresses-openapi.yml\n  - openapi/solidus-labs-tokensniffer-pairs-openapi.yml\n  - openapi/solidus-labs-tokensniffer-tokens-openapi.yml\n  - openapi/solidus-labs-tokensniffer-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/authentication/solidus-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- RegTech
- Trade Surveillance
- Market Integrity
- Transaction Monitoring
- Digital Assets
- Cryptocurrency
- Blockchain
- Token Security
- Scam Detection
- Smart Contracts
- Anti-Money Laundering
- Web3
- DeFi
---
