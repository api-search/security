---
api_key_in:
- header
api_specs:
- filename: zuplo-openapi.yml
  format: yaml
  label: Zuplo Developer API
  slug: zuplo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zuplo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zuplo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zuplo
provider_slug: zuplo
scheme_count: 1
schemes:
- description: 'API key authentication. Format: Bearer {api-key}'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/zuplo-openapi.yml
  type: apiKey
slug: zuplo-authentication
source_filename: zuplo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zuplo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Format: Bearer {api-key}'\n  sources:\n  - openapi/zuplo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/authentication/zuplo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Gateway
- API Management
- Gateways
- Platform
---
