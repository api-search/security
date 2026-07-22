---
api_key_in:
- header
api_specs:
- filename: superform-openapi-original.json
  format: json
  label: Superform API
  slug: superform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-openapi-original.json
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
- Vaults
- Yield Aggregation
- Cross Chain
- Onchain
- Blockchain
- Smart Accounts
---
