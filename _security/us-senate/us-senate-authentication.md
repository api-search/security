---
api_key_in:
- header
api_specs:
- filename: us-senate-lda-openapi.yml
  format: yaml
  label: Senate Lobbying Disclosure Act (LDA) API
  slug: lda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/openapi/us-senate-lda-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Senate Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Senate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: US Senate
provider_slug: us-senate
scheme_count: 1
schemes:
- description: 'Token-based auth. Format: ''Token YOUR_API_KEY'''
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/us-senate-lda-openapi.yml
  type: apiKey
slug: us-senate-authentication
source_filename: us-senate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/us-senate-lda-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based auth. Format: ''Token YOUR_API_KEY'''\n  sources:\n  - openapi/us-senate-lda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-senate/refs/heads/main/authentication/us-senate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Lobbying
- Government Transparency
- Campaign Finance
- Open Data
---
