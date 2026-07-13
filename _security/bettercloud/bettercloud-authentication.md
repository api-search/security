---
api_key_in:
- header
api_specs:
- filename: bettercloud-platform-api.yaml
  format: yaml
  label: BetterCloud Platform API
  slug: bettercloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/openapi/bettercloud-platform-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bettercloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetterCloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BetterCloud
provider_slug: bettercloud
scheme_count: 1
schemes:
- description: API key authentication. Provide your BetterCloud API key in the X-API-Key header. Keys can be generated from the BetterCloud developer portal.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/bettercloud-platform-api.yaml
  type: apiKey
slug: bettercloud-authentication
source_filename: bettercloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bettercloud-platform-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication. Provide your BetterCloud API key in the X-API-Key header.\n    Keys can be generated from the BetterCloud developer portal.\n  sources:\n  - openapi/bettercloud-platform-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/authentication/bettercloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
---
