---
api_key_in:
- header
api_specs:
- filename: agco-agcommand-api-openapi.yml
  format: yaml
  label: AGCO AgCommand API
  slug: agcommand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/openapi/agco-agcommand-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agco Authentication
name_suffix: Authentication
oauth_flows: []
overview: agco secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: agco
provider_slug: agco
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/agco-agcommand-api-openapi.yml
  type: apiKey
slug: agco-authentication
source_filename: agco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agco-agcommand-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/agco-agcommand-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/authentication/agco-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fortune 500
---
