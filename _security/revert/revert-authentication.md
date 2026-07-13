---
api_key_in:
- header
api_specs:
- filename: revert-unified-api-openapi.yml
  format: yaml
  label: Revert Unified API
  slug: revert-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-unified-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revert
provider_slug: revert
scheme_count: 1
schemes:
- description: Your official API key for accessing Revert APIs
  in: header
  name: ApiTokenAuth
  parameter: x-revert-api-token
  sources:
  - openapi/revert-unified-api-openapi.yml
  type: apiKey
slug: revert-authentication
source_filename: revert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revert-unified-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: x-revert-api-token\n  description: Your official API key for accessing Revert APIs\n  sources:\n  - openapi/revert-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/authentication/revert-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Integrations
- CRM
- Unified API
- Open Source
---
