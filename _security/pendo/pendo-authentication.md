---
api_key_in:
- header
api_specs:
- filename: pendo-openapi.yml
  format: yaml
  label: Pendo Engage API
  slug: engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendo/refs/heads/main/openapi/pendo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pendo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pendo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pendo
provider_slug: pendo
scheme_count: 1
schemes:
- description: Per-subscription Pendo integration key issued from the Pendo UI.
  in: header
  name: integrationKey
  parameter: X-Pendo-Integration-Key
  sources:
  - openapi/pendo-openapi.yml
  type: apiKey
slug: pendo-authentication
source_filename: pendo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pendo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: integrationKey\n  type: apiKey\n  in: header\n  parameter: X-Pendo-Integration-Key\n  description: Per-subscription Pendo integration key issued from the Pendo UI.\n  sources:\n  - openapi/pendo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendo/refs/heads/main/authentication/pendo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Product
- Analytics
- In-App Guidance
- Customer Success
- NPS
---
