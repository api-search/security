---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: reservoir-accounts-api-openapi.yml
  format: yaml
  label: Reservoir Accounts API
  slug: reservoir-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-accounts-api-openapi.yml
- filename: reservoir-activity-api-openapi.yml
  format: yaml
  label: Reservoir Activity API
  slug: reservoir-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-activity-api-openapi.yml
- filename: reservoir-attributes-api-openapi.yml
  format: yaml
  label: Reservoir Attributes API
  slug: reservoir-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-attributes-api-openapi.yml
- filename: reservoir-chain-api-openapi.yml
  format: yaml
  label: Reservoir Chain API
  slug: reservoir-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-chain-api-openapi.yml
- filename: reservoir-collections-api-openapi.yml
  format: yaml
  label: Reservoir Collections API
  slug: reservoir-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-collections-api-openapi.yml
- filename: reservoir-events-api-openapi.yml
  format: yaml
  label: Reservoir Events API
  slug: reservoir-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-events-api-openapi.yml
- filename: reservoir-manage-orders-api-openapi.yml
  format: yaml
  label: Reservoir Manage Orders API
  slug: reservoir-manage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-manage-orders-api-openapi.yml
- filename: reservoir-management-api-openapi.yml
  format: yaml
  label: Reservoir Management API
  slug: reservoir-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-management-api-openapi.yml
- filename: reservoir-marketplace-api-openapi.yml
  format: yaml
  label: Reservoir Marketplace API
  slug: reservoir-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-marketplace-api-openapi.yml
- filename: reservoir-misc-api-openapi.yml
  format: yaml
  label: Reservoir Misc API
  slug: reservoir-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-misc-api-openapi.yml
- filename: reservoir-orders-api-openapi.yml
  format: yaml
  label: Reservoir Orders API
  slug: reservoir-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-orders-api-openapi.yml
- filename: reservoir-owners-api-openapi.yml
  format: yaml
  label: Reservoir Owners API
  slug: reservoir-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-owners-api-openapi.yml
- filename: reservoir-redirects-api-openapi.yml
  format: yaml
  label: Reservoir Redirects API
  slug: reservoir-redirects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-redirects-api-openapi.yml
- filename: reservoir-sales-api-openapi.yml
  format: yaml
  label: Reservoir Sales API
  slug: reservoir-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sales-api-openapi.yml
- filename: reservoir-sources-api-openapi.yml
  format: yaml
  label: Reservoir Sources API
  slug: reservoir-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sources-api-openapi.yml
- filename: reservoir-stats-api-openapi.yml
  format: yaml
  label: Reservoir Stats API
  slug: reservoir-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-stats-api-openapi.yml
- filename: reservoir-tokens-api-openapi.yml
  format: yaml
  label: Reservoir Tokens API
  slug: reservoir-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-tokens-api-openapi.yml
- filename: reservoir-transfers-api-openapi.yml
  format: yaml
  label: Reservoir Transfers API
  slug: reservoir-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-transfers-api-openapi.yml
- filename: reservoir-x-deprecated-api-openapi.yml
  format: yaml
  label: Reservoir X Deprecated API
  slug: reservoir-x-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-x-deprecated-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Reservoir Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reservoir secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reservoir
provider_slug: reservoir
scheme_count: 1
schemes:
- in: header
  name: API_KEY
  parameter: x-api-key
  sources:
  - openapi/reservoir-api-openapi.yml
  type: apiKey
slug: reservoir-authentication
source_filename: reservoir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/reservoir-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/reservoir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/authentication/reservoir-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Blockchain
- Marketplace
- Ethereum
- EVM
- Liquidity
- Order Book
- Web3
- DeFi
- Trading
- Data API
---
