---
api_key_in:
- header
api_specs:
- filename: iota-auth-api-openapi.yml
  format: yaml
  label: IOTA auth API
  slug: iota-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-auth-api-openapi.yml
- filename: iota-chains-api-openapi.yml
  format: yaml
  label: IOTA chains API
  slug: iota-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-chains-api-openapi.yml
- filename: iota-coin-query-api-openapi.yml
  format: yaml
  label: IOTA Coin Query API
  slug: iota-coin-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-coin-query-api-openapi.yml
- filename: iota-corecontracts-api-openapi.yml
  format: yaml
  label: IOTA corecontracts API
  slug: iota-corecontracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-corecontracts-api-openapi.yml
- filename: iota-extended-api-openapi.yml
  format: yaml
  label: IOTA Extended API
  slug: iota-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-extended-api-openapi.yml
- filename: iota-governance-api-openapi.yml
  format: yaml
  label: IOTA Governance API
  slug: iota-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-governance-api-openapi.yml
- filename: iota-health-api-openapi.yml
  format: yaml
  label: IOTA Health API
  slug: iota-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-health-api-openapi.yml
- filename: iota-metrics-api-openapi.yml
  format: yaml
  label: IOTA metrics API
  slug: iota-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-metrics-api-openapi.yml
- filename: iota-move-utils-api-openapi.yml
  format: yaml
  label: IOTA Move Utils API
  slug: iota-move-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-move-utils-api-openapi.yml
- filename: iota-node-api-openapi.yml
  format: yaml
  label: IOTA node API
  slug: iota-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-node-api-openapi.yml
- filename: iota-read-api-openapi.yml
  format: yaml
  label: IOTA Read API
  slug: iota-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-read-api-openapi.yml
- filename: iota-requests-api-openapi.yml
  format: yaml
  label: IOTA requests API
  slug: iota-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-requests-api-openapi.yml
- filename: iota-transaction-builder-api-openapi.yml
  format: yaml
  label: IOTA Transaction Builder API
  slug: iota-transaction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-transaction-builder-api-openapi.yml
- filename: iota-users-api-openapi.yml
  format: yaml
  label: IOTA users API
  slug: iota-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-users-api-openapi.yml
- filename: iota-write-api-openapi.yml
  format: yaml
  label: IOTA Write API
  slug: iota-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-write-api-openapi.yml
- filename: iota-ws-api-openapi.yml
  format: yaml
  label: IOTA Ws API
  slug: iota-ws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-ws-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iota Authentication
name_suffix: Authentication
oauth_flows: []
overview: IOTA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IOTA
provider_slug: iota
scheme_count: 1
schemes:
- description: JWT Token
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/iota-evm-wasp-openapi.yaml
  type: apiKey
slug: iota-authentication
source_filename: iota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iota-evm-wasp-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT Token\n  sources:\n  - openapi/iota-evm-wasp-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/authentication/iota-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Distributed Ledger
- Web3
- DeFi
- Cryptocurrency
- Move
- Tangle
---
