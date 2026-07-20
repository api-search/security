---
api_key_in:
- header
api_specs:
- filename: anchorage-v2-openapi-original.yml
  format: yaml
  label: Anchorage Digital REST API v2.0
  slug: anchorage-digital-rest-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/openapi/anchorage-v2-openapi-original.yml
- filename: anchorage-v3-openapi-original.yml
  format: yaml
  label: Anchorage Digital REST API v3
  slug: anchorage-digital-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/openapi/anchorage-v3-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anchorage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anchorage Digital secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anchorage Digital
provider_slug: anchorage
scheme_count: 1
schemes:
- description: An API key associated with a security role
  in: header
  name: Api-Access-Key
  parameter: Api-Access-Key
  sources:
  - openapi/anchorage-v2-openapi-original.yml
  - openapi/anchorage-v3-openapi-original.yml
  type: apiKey
slug: anchorage-authentication
source_filename: anchorage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anchorage-v2-openapi-original.yml, openapi/anchorage-v3-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Api-Access-Key\n  type: apiKey\n  in: header\n  parameter: Api-Access-Key\n  description: An API key associated with a security role\n  sources:\n  - openapi/anchorage-v2-openapi-original.yml\n  - openapi/anchorage-v3-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/authentication/anchorage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Digital Assets
- Custody
- Trading
- Staking
- Settlement
- Stablecoins
- Banking
- Institutional
---
