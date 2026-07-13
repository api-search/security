---
api_key_in:
- header
api_specs:
- filename: ion-group-openapi.yml
  format: yaml
  label: Ion Group Acuris Entities API
  slug: acuris-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ion-group/refs/heads/main/openapi/ion-group-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ion Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ion Group secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ion Group
provider_slug: ion-group
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/ion-group-openapi.yml
  type: apiKey
slug: ion-group-authentication
source_filename: ion-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ion-group-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/ion-group-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ion-group/refs/heads/main/authentication/ion-group-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Financial
- Financial Services
- Trading
---
