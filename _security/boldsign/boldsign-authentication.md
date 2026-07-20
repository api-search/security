---
api_key_in:
- header
api_specs:
- filename: index.html
  format: yaml
  label: BoldSign eSignature API
  slug: boldsign-esignature-api
  spec_type: OpenAPI
  url: https://api.boldsign.com/swagger/index.html
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Boldsign Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoldSign secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BoldSign
provider_slug: boldsign
scheme_count: 2
schemes:
- description: 'Format ''Bearer'' [space] [TOKEN]. Ex: ''Bearer [example key]'''
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/boldsign-esignature-openapi.yml
  type: apiKey
- description: 'Format [API-KEY]. Ex: ''abcdef12345'''
  in: header
  name: X-API-KEY
  parameter: X-API-KEY
  sources:
  - openapi/boldsign-esignature-openapi.yml
  type: apiKey
slug: boldsign-authentication
source_filename: boldsign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boldsign-esignature-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format ''Bearer'' [space] [TOKEN]. Ex: ''Bearer [example key]'''\n  sources:\n  - openapi/boldsign-esignature-openapi.yml\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: 'Format [API-KEY]. Ex: ''abcdef12345'''\n  sources:\n  - openapi/boldsign-esignature-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boldsign/refs/heads/main/authentication/boldsign-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- E-Signature
- Electronic Signature
- Document Management
- Embedded Signing
- Webhooks
- Templates
- Identity Verification
- Compliance
---
