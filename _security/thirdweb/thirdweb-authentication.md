---
api_key_in:
- header
api_specs:
- filename: thirdweb-authentication-api-openapi.yml
  format: yaml
  label: thirdweb Authentication API
  slug: thirdweb-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-authentication-api-openapi.yml
- filename: thirdweb-contracts-api-openapi.yml
  format: yaml
  label: thirdweb Contracts API
  slug: thirdweb-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-contracts-api-openapi.yml
- filename: thirdweb-engine-api-openapi.yml
  format: yaml
  label: thirdweb Engine API
  slug: thirdweb-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-engine-api-openapi.yml
- filename: thirdweb-insight-api-openapi.yml
  format: yaml
  label: thirdweb Insight API
  slug: thirdweb-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-insight-api-openapi.yml
- filename: thirdweb-nebula-api-openapi.yml
  format: yaml
  label: thirdweb Nebula API
  slug: thirdweb-nebula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-nebula-api-openapi.yml
- filename: thirdweb-payments-api-openapi.yml
  format: yaml
  label: thirdweb Payments API
  slug: thirdweb-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-payments-api-openapi.yml
- filename: thirdweb-tokens-api-openapi.yml
  format: yaml
  label: thirdweb Tokens API
  slug: thirdweb-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-tokens-api-openapi.yml
- filename: thirdweb-transactions-api-openapi.yml
  format: yaml
  label: thirdweb Transactions API
  slug: thirdweb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-transactions-api-openapi.yml
- filename: thirdweb-wallets-api-openapi.yml
  format: yaml
  label: thirdweb Wallets API
  slug: thirdweb-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-wallets-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thirdweb Authentication
name_suffix: Authentication
oauth_flows: []
overview: thirdweb secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: thirdweb
provider_slug: thirdweb
scheme_count: 4
schemes:
- description: Client ID for frontend usage. Web sends x-client-id only; native apps also send x-bundle-id.
  in: header
  name: ClientAuth
  parameter: x-client-id
  sources:
  - openapi/thirdweb-openapi.yml
  type: apiKey
- description: Bundle ID for native (desktop/mobile) platform authentication alongside x-client-id.
  in: header
  name: BundleIdAuth
  parameter: x-bundle-id
  sources:
  - openapi/thirdweb-openapi.yml
  type: apiKey
- description: Secret key for backend usage; never expose publicly.
  in: header
  name: SecretKeyAuth
  parameter: x-secret-key
  sources:
  - openapi/thirdweb-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT access token obtained from wallet authentication, for frontend usage.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/thirdweb-openapi.yml
  type: http
slug: thirdweb-authentication
source_filename: thirdweb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thirdweb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ClientAuth\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  description: Client ID for frontend usage. Web sends x-client-id only; native apps also send\n    x-bundle-id.\n  sources:\n  - openapi/thirdweb-openapi.yml\n- name: BundleIdAuth\n  type: apiKey\n  in: header\n  parameter: x-bundle-id\n  description: Bundle ID for native (desktop/mobile) platform authentication alongside x-client-id.\n  sources:\n  - openapi/thirdweb-openapi.yml\n- name: SecretKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-secret-key\n  description: Secret key for backend usage; never expose publicly.\n  sources:\n  - openapi/thirdweb-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token obtained from wallet authentication, for frontend usage.\n  sources:\n\
  \  - openapi/thirdweb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/authentication/thirdweb-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Web3
- Blockchain
- Wallets
- Smart Contracts
- Payments
- Indexer
---
