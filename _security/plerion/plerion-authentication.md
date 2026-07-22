---
api_key_in: []
api_specs:
- filename: plerion-openapi-original.yml
  format: yaml
  label: Plerion API
  slug: plerion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plerion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plerion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plerion
provider_slug: plerion
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: Bearer API Key. For example, "Bearer {Tenant API Key}"
  docs: https://docs.plerion.com/api-reference/index
  key_management: https://app.plerion.com/settings/api-keys
  name: APIKey
  scheme: bearer
  sources:
  - openapi/plerion-openapi-original.yml
  type: http
slug: plerion-authentication
source_filename: plerion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/plerion-openapi-original.yml\ndocs: https://docs.plerion.com/api-reference/index\nkey_management: https://app.plerion.com/settings/api-keys\nsummary:\n  types:\n  - http\n  model: Tenant API Key sent as an HTTP Bearer token\n  header: 'Authorization: Bearer $PLERION_API_KEY'\n  transport: HTTPS required (plain HTTP requests fail)\nschemes:\n- name: APIKey\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: Bearer API Key. For example, \"Bearer {Tenant API Key}\"\n  docs: https://docs.plerion.com/api-reference/index\n  key_management: https://app.plerion.com/settings/api-keys\n  sources:\n  - openapi/plerion-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/authentication/plerion-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cloud Security
- CSPM
- Cloud Workload Protection
- Vulnerability Management
- Compliance
- AI Security
- DevSecOps
- API
---
