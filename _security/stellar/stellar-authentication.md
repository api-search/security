---
api_key_in:
- header
- query
api_specs:
- filename: stellar-horizon-api.yml
  format: yaml
  label: Stellar Horizon API
  slug: horizon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-horizon-api.yml
- filename: stellar-anchor-platform-api.yml
  format: yaml
  label: Stellar Anchor Platform API
  slug: anchor-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-anchor-platform-api.yml
- filename: stellar-disbursement-platform-api.yml
  format: yaml
  label: Stellar Disbursement Platform API
  slug: disbursement-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/openapi/stellar-disbursement-platform-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stellar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stellar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stellar
provider_slug: stellar
scheme_count: 2
schemes:
- description: Authorization header containing an SDP JWT (ES256) or an SDP_ API key.
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/stellar-disbursement-platform-api.yml
  type: apiKey
- description: Query parameter containing a SEP-24 JWT.
  in: query
  name: SEP24QueryAuth
  parameter: token
  sources:
  - openapi/stellar-disbursement-platform-api.yml
  type: apiKey
slug: stellar-authentication
source_filename: stellar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stellar-disbursement-platform-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header containing an SDP JWT (ES256) or an SDP_ API key.\n  sources:\n  - openapi/stellar-disbursement-platform-api.yml\n- name: SEP24QueryAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Query parameter containing a SEP-24 JWT.\n  sources:\n  - openapi/stellar-disbursement-platform-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellar/refs/heads/main/authentication/stellar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Blockchain
- Cryptocurrency
- Decentralized Exchange
- Ledger
- Payments
- Smart Contracts
- Web3
---
