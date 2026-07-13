---
api_key_in:
- header
api_specs:
- filename: click-and-drop-api-v1.yaml
  format: yaml
  label: Royal Mail Click & Drop API
  slug: royal-mail-click-drop-api
  spec_type: OpenAPI
  url: https://api.parcel.royalmail.com/doc/v1/click-and-drop-api-v1.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Royal Mail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Royal Mail secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Royal Mail
provider_slug: royal-mail
scheme_count: 1
schemes:
- description: Authorization header using the Bearer scheme. Enter 'Bearer [space] and then your token.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/click-and-drop-api-v1.yml
  type: apiKey
slug: royal-mail-authentication
source_filename: royal-mail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/click-and-drop-api-v1.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header using the Bearer scheme. Enter 'Bearer [space] and then\n    your token.\n  sources:\n  - openapi/click-and-drop-api-v1.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/royal-mail/refs/heads/main/authentication/royal-mail-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Shipping
- Postal Services
- Labels
- Tracking
- Logistics
- Barcodes
- Click and Drop
- UK
---
