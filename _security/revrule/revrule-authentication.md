---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Revrule Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevRule by Payload secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RevRule by Payload
provider_slug: revrule
scheme_count: 1
schemes:
- description: Bearer API key for authenticated endpoints
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/revrule-openapi.yml
  type: apiKey
slug: revrule-authentication
source_filename: revrule-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/revrule-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer API key for authenticated endpoints\n  sources:\n  - openapi/revrule-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revrule/refs/heads/main/authentication/revrule-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Revenue
- Payments
- API
- FinTech
---
