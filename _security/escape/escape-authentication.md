---
api_key_in:
- header
api_specs:
- filename: escape-openapi.yml
  format: yaml
  label: Escape Public API
  slug: escape-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Escape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Escape secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Escape
provider_slug: escape
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-ESCAPE-API-KEY
  sources:
  - openapi/escape-openapi.yml
  type: apiKey
slug: escape-authentication
source_filename: escape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/escape-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-ESCAPE-API-KEY\n  sources:\n  - openapi/escape-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/authentication/escape-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Platform
- Security
---
