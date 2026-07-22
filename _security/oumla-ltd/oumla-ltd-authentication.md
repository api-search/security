---
api_key_in:
- header
api_specs:
- filename: oumla-ltd-openapi-original.json
  format: json
  label: Oumla Core Server API
  slug: oumla-core-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oumla Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oumla Ltd secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oumla Ltd
provider_slug: oumla-ltd
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/oumla-ltd-openapi-original.json
  type: apiKey
slug: oumla-ltd-authentication
source_filename: oumla-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oumla-ltd-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication\n  sources:\n  - openapi/oumla-ltd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/authentication/oumla-ltd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Digital Assets
- Wallet Infrastructure
- Custody
- Tokenization
- Smart Contracts
- Web3
- Fintech
- Saudi Arabia
---
