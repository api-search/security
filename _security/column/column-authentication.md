---
api_key_in: []
api_specs:
- filename: column-asyncapi.yml
  format: yaml
  label: Column Webhooks
  slug: column-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/openapi/column-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Column Authentication
name_suffix: Authentication
oauth_flows: []
overview: Column secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Column
provider_slug: column
scheme_count: 1
schemes:
- description: Column uses HTTP Basic Auth with your API key as the username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/column-openapi.yml
  type: http
slug: column-authentication
source_filename: column-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/column-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Column uses HTTP Basic Auth with your API key as the username.\n  sources:\n  - openapi/column-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column/refs/heads/main/authentication/column-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- Banking
- BaaS
- ACH
- Wires
---
