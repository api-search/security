---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Trading 212 Public API
  slug: trading-212-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trading212/refs/heads/main/openapi/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trading212 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trading 212 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trading 212
provider_slug: trading212
scheme_count: 2
schemes:
- description: Use your API Key as the username and your API Secret as the password
  name: authWithSecretKey
  scheme: basic
  sources:
  - openapi/openapi.yaml
  type: http
- in: header
  name: legacyApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: trading212-authentication
source_filename: trading212-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: authWithSecretKey\n  type: http\n  scheme: basic\n  description: Use your API Key as the username and your API Secret as the password\n  sources:\n  - openapi/openapi.yaml\n- name: legacyApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trading212/refs/heads/main/authentication/trading212-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Investing
- Finance
- Trading
- Stocks
- Portfolio
- Commission-Free
- ISA
---
