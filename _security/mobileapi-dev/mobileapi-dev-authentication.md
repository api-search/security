---
api_key_in:
- header
- query
api_specs:
- filename: mobileapi-openapi.yml
  format: yaml
  label: MobileAPI
  slug: mobileapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mobileapi Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: MobileAPI.dev secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MobileAPI.dev
provider_slug: mobileapi-dev
scheme_count: 2
schemes:
- description: Provide your API key in the Authorization header using either 'Token YOUR_API_KEY' or 'Bearer [example key]'. Both formats are equivalent.
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/mobileapi-openapi.yml
  type: apiKey
- description: Fallback - supply your API key as the 'key' query parameter.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/mobileapi-openapi.yml
  type: apiKey
slug: mobileapi-dev-authentication
source_filename: mobileapi-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mobileapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide your API key in the Authorization header using either 'Token YOUR_API_KEY'\n    or 'Bearer [example key]'. Both formats are equivalent.\n  sources:\n  - openapi/mobileapi-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Fallback - supply your API key as the 'key' query parameter.\n  sources:\n  - openapi/mobileapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/authentication/mobileapi-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data API
- Developer Tools
- Device Specifications
- Mobile Data
- Phone Specs
- REST API
- SaaS
---
