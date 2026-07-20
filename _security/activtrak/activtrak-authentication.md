---
api_key_in:
- header
api_specs:
- filename: activtrak-openapi-original.yaml
  format: yaml
  label: ActivTrak Public APIs
  slug: activtrak-public-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activtrak/refs/heads/main/openapi/activtrak-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Activtrak Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActivTrak secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActivTrak
provider_slug: activtrak
scheme_count: 1
schemes:
- description: 'Public API key sent in the x-api-key header. Some endpoints also accept `Authorization: Bearer {apiKey}`. Keys are created in the ActivTrak app under API & Integrations > API Keys.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/activtrak-openapi-original.yaml
  type: apiKey
slug: activtrak-authentication
source_filename: activtrak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/activtrak-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Public API key sent in the x-api-key header. Some endpoints also accept `Authorization:\n    Bearer {apiKey}`. Keys are created in the ActivTrak app under API & Integrations > API Keys.'\n  sources:\n  - openapi/activtrak-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activtrak/refs/heads/main/authentication/activtrak-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Saas
- Workforce Analytics
- Productivity
- Employee Monitoring
- Workforce Management
- SCIM
- Reporting
---
