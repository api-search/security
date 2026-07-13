---
api_key_in: []
api_specs:
- filename: nudge-security-openapi.yml
  format: yaml
  label: Nudge Security API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nudge Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nudge Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nudge Security
provider_slug: nudge-security
scheme_count: 1
schemes:
- bearerFormat: API Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nudge-security-openapi.yml
  type: http
slug: nudge-security-authentication
source_filename: nudge-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nudge-security-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  sources:\n  - openapi/nudge-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/authentication/nudge-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- AI Security
- Compliance
- Governance
- OAuth
- SaaS Management
- SaaS Security
- Security
- Shadow IT
- SSPM
---
