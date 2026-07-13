---
api_key_in:
- header
- query
api_specs:
- filename: minerstat-openapi.yml
  format: yaml
  label: Minerstat
  slug: minerstat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minerstat/refs/heads/main/openapi/minerstat-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Minerstat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minerstat secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Minerstat
provider_slug: minerstat
scheme_count: 2
schemes:
- description: Recommended authentication using the X-API-Key header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/minerstat-openapi.yml
  type: apiKey
- description: Alternative authentication using the key query parameter.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/minerstat-openapi.yml
  type: apiKey
slug: minerstat-authentication
source_filename: minerstat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/minerstat-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Recommended authentication using the X-API-Key header.\n  sources:\n  - openapi/minerstat-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Alternative authentication using the key query parameter.\n  sources:\n  - openapi/minerstat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minerstat/refs/heads/main/authentication/minerstat-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Mining
- Cryptocurrency
- Mining Pools
---
