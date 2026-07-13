---
api_key_in: []
api_specs:
- filename: regulatory-openapi.yml
  format: yaml
  label: FINRA Developer Center API
  slug: finra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulatory/refs/heads/main/openapi/regulatory-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Regulatory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regulatory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Regulatory
provider_slug: regulatory
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token issued by FINRA Identity Provider.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/regulatory-openapi.yml
  type: http
slug: regulatory-authentication
source_filename: regulatory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regulatory-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token issued by FINRA Identity Provider.\n  sources:\n  - openapi/regulatory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulatory/refs/heads/main/authentication/regulatory-authentication.yml
summary_line: http · 1 scheme
tags:
- Compliance
- Financial Services
- Governance
- Healthcare Regulation
- Regulatory Reporting
- Risk Management
- RegTech
---
