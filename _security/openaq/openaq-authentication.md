---
api_key_in:
- header
api_specs:
- filename: openaq-openapi.yml
  format: yaml
  label: OpenAQ
  slug: openaq
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openaq/refs/heads/main/openapi/openaq-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openaq Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenAQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenAQ
provider_slug: openaq
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/openaq-openapi.yml
  type: apiKey
slug: openaq-authentication
source_filename: openaq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openaq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/openaq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openaq/refs/heads/main/authentication/openaq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data
- Data Quality
---
