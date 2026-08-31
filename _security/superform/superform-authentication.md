---
api_key_in:
- header
api_specs:
- filename: superform-auxiliary-api-openapi.yml
  format: yaml
  label: Superform Auxiliary API
  slug: superform-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-auxiliary-api-openapi.yml
- filename: superform-balances-api-openapi.yml
  format: yaml
  label: Superform Balances API
  slug: superform-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-balances-api-openapi.yml
- filename: superform-contract-checker-api-openapi.yml
  format: yaml
  label: Superform Contract Checker API
  slug: superform-contract-checker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-contract-checker-api-openapi.yml
- filename: superform-data-api-openapi.yml
  format: yaml
  label: Superform Data API
  slug: superform-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-data-api-openapi.yml
- filename: superform-execution-api-openapi.yml
  format: yaml
  label: Superform Execution API
  slug: superform-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-execution-api-openapi.yml
- filename: superform-explorer-api-openapi.yml
  format: yaml
  label: Superform Explorer API
  slug: superform-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-explorer-api-openapi.yml
- filename: superform-health-api-openapi.yml
  format: yaml
  label: Superform Health API
  slug: superform-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-health-api-openapi.yml
- filename: superform-migrate-api-openapi.yml
  format: yaml
  label: Superform Migrate API
  slug: superform-migrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-migrate-api-openapi.yml
- filename: superform-protocol-api-openapi.yml
  format: yaml
  label: Superform Protocol API
  slug: superform-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-protocol-api-openapi.yml
- filename: superform-protocol-rewards-api-openapi.yml
  format: yaml
  label: Superform Protocol Rewards API
  slug: superform-protocol-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-protocol-rewards-api-openapi.yml
- filename: superform-simulator-api-openapi.yml
  format: yaml
  label: Superform Simulator API
  slug: superform-simulator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-simulator-api-openapi.yml
- filename: superform-stats-api-openapi.yml
  format: yaml
  label: Superform Stats API
  slug: superform-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-stats-api-openapi.yml
- filename: superform-superrewardsapi-api-openapi.yml
  format: yaml
  label: Superform SuperRewardsAPI API
  slug: superform-superrewardsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-superrewardsapi-api-openapi.yml
- filename: superform-token-distribution-api-openapi.yml
  format: yaml
  label: Superform Token Distribution API
  slug: superform-token-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-token-distribution-api-openapi.yml
- filename: superform-vault-api-openapi.yml
  format: yaml
  label: Superform Vault API
  slug: superform-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-vault-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Superform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superform secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Superform
provider_slug: superform
scheme_count: 1
schemes:
- description: Provide the api key issued to you
  in: header
  name: apiKey
  parameter: SF-API-KEY
  sources:
  - openapi/superform-openapi-original.json
  type: apiKey
slug: superform-authentication
source_filename: superform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/superform-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: SF-API-KEY\n  description: Provide the api key issued to you\n  sources:\n  - openapi/superform-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/authentication/superform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Defi Yield
- DeFi
- Vault
- Yield Aggregation
- Cross Chain
- Onchain
- Blockchain
- Smart Accounts
---
