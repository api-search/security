---
api_key_in:
- header
api_specs:
- filename: clusters-v1-openapi.yml
  format: yaml
  label: Clusters API v1
  slug: clusters-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-v1-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Clusters Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clusters secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clusters
provider_slug: clusters
scheme_count: 2
schemes:
- description: Optional API key from https://clusters.xyz/developer to raise rate limits.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/clusters-v1-openapi.yml
  type: apiKey
- description: Wallet-signature auth token obtained from POST /auth/token.
  name: WalletBearerAuth
  scheme: bearer
  sources:
  - openapi/clusters-v1-openapi.yml
  type: http
slug: clusters-authentication
source_filename: clusters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clusters-v1-openapi.yml\ndocs: https://docs.clusters.xyz/getting-started/api/v1/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Optional API key from https://clusters.xyz/developer to raise rate limits.\n  sources:\n  - openapi/clusters-v1-openapi.yml\n- name: WalletBearerAuth\n  type: http\n  scheme: bearer\n  description: Wallet-signature auth token obtained from POST /auth/token.\n  sources:\n  - openapi/clusters-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/authentication/clusters-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Infrastructure
- Identity
- Naming
- Blockchain
- Web3
- Wallet
- Multichain
- Resolver
---
