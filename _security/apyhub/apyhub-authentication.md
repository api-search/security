---
api_key_in:
- header
api_specs:
- filename: apyhub-openapi.yaml
  format: yaml
  label: ApyHub API
  slug: apyhub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/openapi/apyhub-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apyhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: ApyHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ApyHub
provider_slug: apyhub
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: apy-token
  sources:
  - openapi/apyhub-openapi.yaml
  type: apiKey
slug: apyhub-authentication
source_filename: apyhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apyhub-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apy-token\n  sources:\n  - openapi/apyhub-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/authentication/apyhub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Platform
- Data Processing
- Document Conversion
- Utility APIs
---
