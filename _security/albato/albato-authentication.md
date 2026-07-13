---
api_key_in:
- header
api_specs:
- filename: albato-automations-openapi.yaml
  format: yaml
  label: Albato Automations API
  slug: automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/openapi/albato-automations-openapi.yaml
- filename: albato-embedded-openapi.yaml
  format: yaml
  label: Albato Embedded API
  slug: embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/openapi/albato-embedded-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Albato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Albato secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Albato
provider_slug: albato
scheme_count: 1
schemes:
- description: Albato account API key
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/albato-automations-openapi.yaml
  - openapi/albato-embedded-openapi.yaml
  type: apiKey
slug: albato-authentication
source_filename: albato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/albato-automations-openapi.yaml, openapi/albato-embedded-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Albato account API key\n  sources:\n  - openapi/albato-automations-openapi.yaml\n  - openapi/albato-embedded-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/authentication/albato-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
---
