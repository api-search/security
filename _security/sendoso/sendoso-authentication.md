---
api_key_in:
- header
api_specs:
- filename: sendoso-api-openapi.yml
  format: yaml
  label: Sendoso Sending Platform API
  slug: sendoso-sending-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/main/openapi/sendoso-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sendoso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendoso secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sendoso
provider_slug: sendoso
scheme_count: 1
schemes:
- description: Sendoso API key from Settings > API Keys
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/sendoso-api-openapi.yml
  type: apiKey
slug: sendoso-authentication
source_filename: sendoso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendoso-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Sendoso API key from Settings > API Keys\n  sources:\n  - openapi/sendoso-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/authentication/sendoso-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Corporate Gifting
- Direct Mail
- Sales Engagement
- Marketing Automation
- CRM Integration
---
