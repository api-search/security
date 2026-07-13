---
api_key_in:
- query
api_specs:
- filename: betsolutions-wallet-api.yaml
  format: yaml
  label: BetSolutions Wallet API
  slug: wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/openapi/betsolutions-wallet-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Betsolutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetSolutions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BetSolutions
provider_slug: betsolutions
scheme_count: 1
schemes:
- description: SHA-256 hash of concatenated request parameters using pipe (|) separator and merchant secret key for request signing.
  in: query
  name: sha256Auth
  parameter: hash
  sources:
  - openapi/betsolutions-wallet-api.yaml
  type: apiKey
slug: betsolutions-authentication
source_filename: betsolutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/betsolutions-wallet-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: sha256Auth\n  type: apiKey\n  in: query\n  parameter: hash\n  description: SHA-256 hash of concatenated request parameters using pipe (|) separator and\n    merchant secret key for request signing.\n  sources:\n  - openapi/betsolutions-wallet-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/authentication/betsolutions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
---
