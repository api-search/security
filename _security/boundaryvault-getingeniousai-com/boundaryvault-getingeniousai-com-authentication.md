---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: BoundaryVault (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoundaryVault (Ingenious AI) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BoundaryVault (Ingenious AI)
provider_slug: boundaryvault-getingeniousai-com
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boundaryvault-getingeniousai-com-openapi.json
  type: http
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/boundaryvault-getingeniousai-com-openapi.json
  type: apiKey
slug: boundaryvault-getingeniousai-com-authentication
source_filename: boundaryvault-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/boundaryvault-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/boundaryvault-getingeniousai-com-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/boundaryvault-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/boundaryvault-getingeniousai-com/authentication/boundaryvault-getingeniousai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Security
- Artificial Intelligence
- Zero Trust
- Compliance
---
