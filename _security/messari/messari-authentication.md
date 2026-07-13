---
api_key_in:
- header
api_specs:
- filename: messari-openapi.yml
  format: yaml
  label: Messari REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Messari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messari secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Messari
provider_slug: messari
scheme_count: 1
schemes:
- description: Messari API key
  in: header
  name: apiKeyAuth
  parameter: x-messari-api-key
  sources:
  - openapi/messari-openapi.yml
  type: apiKey
slug: messari-authentication
source_filename: messari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/messari-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-messari-api-key\n  description: Messari API key\n  sources:\n  - openapi/messari-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/authentication/messari-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- Research
- Analytics
- Asset Data
- Fundamentals
- News
- Token Unlocks
---
