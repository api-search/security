---
api_key_in:
- header
api_specs:
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb API
  slug: thirdweb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb Engine
  slug: thirdweb-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb Insight
  slug: thirdweb-insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb Nebula
  slug: thirdweb-nebula
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb Payments and Bridge
  slug: thirdweb-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
- filename: thirdweb-openapi.yml
  format: yaml
  label: thirdweb RPC Edge
  slug: thirdweb-rpc-edge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-openapi.yml
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
