---
api_key_in:
- header
api_specs:
- filename: document360-document360-api-openapi.yml
  format: yaml
  label: Document360 API
  slug: document360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/openapi/document360-document360-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Document360 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Document360 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Document360
provider_slug: document360
scheme_count: 1
schemes:
- in: header
  name: apiToken
  parameter: api_token
  sources:
  - openapi/document360-document360-api-openapi.yml
  type: apiKey
slug: document360-authentication
source_filename: document360-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/document360-document360-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: api_token\n  sources:\n  - openapi/document360-document360-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/authentication/document360-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Documentation
- Knowledge Base
- SaaS
---
