---
api_key_in:
- header
api_specs:
- filename: saas-alerts-openapi.yml
  format: yaml
  label: SaaS Alerts API
  slug: saas-alerts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/openapi/saas-alerts-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Saas Alerts Authentication
name_suffix: Authentication
oauth_flows: []
overview: SaaS Alerts secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SaaS Alerts
provider_slug: saas-alerts
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/saas-alerts-openapi.yml
  type: apiKey
slug: saas-alerts-authentication
source_filename: saas-alerts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/saas-alerts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/saas-alerts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/authentication/saas-alerts-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- MSP
- SaaS Security
- Security Monitoring
- Threat Detection
- Microsoft 365
- Google Workspace
- MSSP
---
