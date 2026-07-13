---
api_key_in:
- header
api_specs:
- filename: spanning-google-workspace-api-openapi.yml
  format: yaml
  label: Spanning Backup for Google Workspace API
  slug: spanning-google-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spanning/refs/heads/main/openapi/spanning-google-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spanning Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spanning secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spanning
provider_slug: spanning
scheme_count: 1
schemes:
- description: Spanning API token obtained from Settings > Backup and Security > API Token in the admin portal
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/spanning-google-workspace-api-openapi.yml
  type: apiKey
slug: spanning-authentication
source_filename: spanning-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spanning-google-workspace-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Spanning API token obtained from Settings > Backup and Security > API Token in\n    the admin portal\n  sources:\n  - openapi/spanning-google-workspace-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spanning/refs/heads/main/authentication/spanning-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Protection
- SaaS Backup
- Cloud Backup
- Microsoft 365
- Google Workspace
- Salesforce
---
