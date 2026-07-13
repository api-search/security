---
api_key_in:
- header
api_specs:
- filename: harness-platform-api.yaml
  format: yaml
  label: Harness Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-platform-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harness Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harness secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harness
provider_slug: harness
scheme_count: 1
schemes:
- description: Harness API key.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/harness-platform-api.yaml
  type: apiKey
slug: harness-authentication
source_filename: harness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harness-platform-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Harness API key.\n  sources:\n  - openapi/harness-platform-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/authentication/harness-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- GitOps
- Internal Developer Portal
- Lifecycle
- Software Delivery
---
