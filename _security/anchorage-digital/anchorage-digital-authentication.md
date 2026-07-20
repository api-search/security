---
api_key_in:
- header
api_specs:
- filename: anchorage-digital-openapi-original.json
  format: json
  label: Anchorage Digital API
  slug: anchorage-digital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage-digital/refs/heads/main/openapi/anchorage-digital-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anchorage Digital Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anchorage Digital secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anchorage Digital
provider_slug: anchorage-digital
scheme_count: 1
schemes:
- description: An API key associated with a security role
  in: header
  name: Api-Access-Key
  parameter: Api-Access-Key
  sources:
  - openapi/anchorage-digital-openapi-original.json
  type: apiKey
slug: anchorage-digital-authentication
source_filename: anchorage-digital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anchorage-digital-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Api-Access-Key\n  type: apiKey\n  in: header\n  parameter: Api-Access-Key\n  description: An API key associated with a security role\n  sources:\n  - openapi/anchorage-digital-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorage-digital/refs/heads/main/authentication/anchorage-digital-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Custody
- Digital Assets
- Banking
- Trading
- Staking
- Settlement
- Institutional
- Blockchain
- Stablecoins
---
