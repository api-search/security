---
api_key_in:
- header
api_specs:
- filename: breeze-admin-api-openapi.yml
  format: yaml
  label: Breeze Admin API
  slug: breeze-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-admin-api-openapi.yml
- filename: breeze-deposits-api-openapi.yml
  format: yaml
  label: Breeze Deposits API
  slug: breeze-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-deposits-api-openapi.yml
- filename: breeze-fund-api-openapi.yml
  format: yaml
  label: Breeze fund API
  slug: breeze-fund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-fund-api-openapi.yml
- filename: breeze-funds-api-openapi.yml
  format: yaml
  label: Breeze Funds API
  slug: breeze-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-funds-api-openapi.yml
- filename: breeze-global-config-api-openapi.yml
  format: yaml
  label: Breeze Global Config API
  slug: breeze-global-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-global-config-api-openapi.yml
- filename: breeze-organization-api-keys-api-openapi.yml
  format: yaml
  label: Breeze Organization API Keys API
  slug: breeze-organization-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-api-keys-api-openapi.yml
- filename: breeze-organization-api-openapi.yml
  format: yaml
  label: Breeze Organization API
  slug: breeze-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-api-openapi.yml
- filename: breeze-organization-funds-api-openapi.yml
  format: yaml
  label: Breeze Organization Funds API
  slug: breeze-organization-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-funds-api-openapi.yml
- filename: breeze-organization-settings-api-openapi.yml
  format: yaml
  label: Breeze Organization Settings API
  slug: breeze-organization-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-organization-settings-api-openapi.yml
- filename: breeze-selective-yield-sources-api-openapi.yml
  format: yaml
  label: Breeze Selective Yield Sources API
  slug: breeze-selective-yield-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-selective-yield-sources-api-openapi.yml
- filename: breeze-strategies-api-openapi.yml
  format: yaml
  label: Breeze Strategies API
  slug: breeze-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-strategies-api-openapi.yml
- filename: breeze-strategy-api-openapi.yml
  format: yaml
  label: Breeze Strategy API
  slug: breeze-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-strategy-api-openapi.yml
- filename: breeze-user-data-api-openapi.yml
  format: yaml
  label: Breeze User Data API
  slug: breeze-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-user-data-api-openapi.yml
- filename: breeze-withdrawals-api-openapi.yml
  format: yaml
  label: Breeze Withdrawals API
  slug: breeze-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-withdrawals-api-openapi.yml
- filename: breeze-yield-sources-api-openapi.yml
  format: yaml
  label: Breeze Yield Sources API
  slug: breeze-yield-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-yield-sources-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Breeze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breeze secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Breeze
provider_slug: breeze
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/breeze-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/breeze-openapi-original.json
  type: http
slug: breeze-authentication
source_filename: breeze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/breeze-openapi-original.json\ndocs: https://docs.breeze.baby/get-your-api-key/instruction\nnotes: >-\n  Integration endpoints authenticate with an API key in the x-api-key header\n  (generated in the Breeze Customer Portal, portal.breeze.baby). Organization and\n  admin endpoints use a JWT bearer token. The x402 Agent Kit path is keyless,\n  gated by USDC micropayments instead.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/breeze-openapi-original.json\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/breeze-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/authentication/breeze-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto Web3
- Solana
- Yield
- DeFi
- Payments
- Blockchain
- AI Agents
---
