---
api_key_in:
- header
api_specs:
- filename: apinizer-api.yaml
  format: yaml
  label: Apinizer API
  slug: apinizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/openapi/apinizer-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apinizer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apinizer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apinizer
provider_slug: apinizer
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/apinizer-api.yaml
  type: apiKey
slug: apinizer-authentication
source_filename: apinizer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apinizer-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/apinizer-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apinizer/refs/heads/main/authentication/apinizer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Gateway
- API Management
- API Monitoring
- API Security
- Policies
---
