---
api_key_in:
- header
api_specs:
- filename: albato-automations-openapi.yaml
  format: yaml
  label: Albato Automations API
  slug: automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/openapi/albato-automations-openapi.yaml
- filename: albato-connections-openapi.yaml
  format: yaml
  label: Albato Connections API
  slug: connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/openapi/albato-connections-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Albato A Single No Code Platform For All Automations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Albato A Single No Code Platform For All Automations secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
scheme_count: 1
schemes:
- description: API key for Albato account access
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/albato-automations-openapi.yaml
  - openapi/albato-connections-openapi.yaml
  type: apiKey
slug: albato-a-single-no-code-platform-for-all-automations-authentication
source_filename: albato-a-single-no-code-platform-for-all-automations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/albato-automations-openapi.yaml, openapi/albato-connections-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for Albato account access\n  sources:\n  - openapi/albato-automations-openapi.yaml\n  - openapi/albato-connections-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/authentication/albato-a-single-no-code-platform-for-all-automations-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
---
