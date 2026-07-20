---
api_key_in:
- header
api_specs:
- filename: blockaid-openapi-original.yml
  format: yaml
  label: Blockaid API
  slug: blockaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockaid/refs/heads/main/openapi/blockaid-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blockaid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockaid secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blockaid
provider_slug: blockaid
scheme_count: 3
schemes:
- in: header
  name: APIKey
  parameter: X-API-Key
  sources:
  - openapi/blockaid-openapi-original.yml
  type: apiKey
- in: header
  name: ClientID
  parameter: X-CLIENT-ID
  sources:
  - openapi/blockaid-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is your auth token. See [API Authentication](/docs/api-reference/before-you-begin/api-authentication) for how to retrieve it.
  name: JWT
  scheme: bearer
  sources:
  - openapi/blockaid-openapi-original.yml
  type: http
slug: blockaid-authentication
source_filename: blockaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/blockaid-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/blockaid-openapi-original.yml\n- name: ClientID\n  type: apiKey\n  in: header\n  parameter: X-CLIENT-ID\n  sources:\n  - openapi/blockaid-openapi-original.yml\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is\n    your auth token. See [API Authentication](/docs/api-reference/before-you-begin/api-authentication)\n    for how to retrieve it.\n  sources:\n  - openapi/blockaid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockaid/refs/heads/main/authentication/blockaid-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Fintech
- Web3 Security
- Blockchain
- Crypto
- Fraud Prevention
- Transaction Scanning
- Wallet Security
- Compliance
- Threat Detection
---
