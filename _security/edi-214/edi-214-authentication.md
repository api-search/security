---
api_key_in:
- header
api_specs:
- filename: stedi-edi214-openapi.yml
  format: yaml
  label: EDI 214 Transportation Carrier Shipment Status Message
  slug: edi-214-standard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edi-214/refs/heads/main/openapi/stedi-edi214-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Edi 214 Authentication
name_suffix: Authentication
oauth_flows: []
overview: edi-214 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: edi-214
provider_slug: edi-214
scheme_count: 1
schemes:
- description: API key in format "Key {your_api_key}" for Stedi platform access
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/stedi-edi214-openapi.yml
  type: apiKey
slug: edi-214-authentication
source_filename: edi-214-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stedi-edi214-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key in format \"Key {your_api_key}\" for Stedi platform access\n  sources:\n  - openapi/stedi-edi214-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edi-214/refs/heads/main/authentication/edi-214-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
