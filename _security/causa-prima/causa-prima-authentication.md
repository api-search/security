---
api_key_in: []
api_specs:
- filename: causa-prima-scribo-openapi.json
  format: json
  label: Scribo Invoice API
  slug: causa-prima-scribo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/causa-prima/refs/heads/main/openapi/causa-prima-scribo-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Causa Prima Authentication
name_suffix: Authentication
oauth_flows: []
overview: Causa Prima secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Causa Prima
provider_slug: causa-prima
scheme_count: 1
schemes:
- description: Optional API key for elevated quotas. Unauthenticated requests are accepted and rate-limited per IP.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/causa-prima-scribo-openapi.json
  type: http
slug: causa-prima-authentication
source_filename: causa-prima-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/causa-prima-scribo-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional API key for elevated quotas. Unauthenticated requests are accepted and\n    rate-limited per IP.\n  sources:\n  - openapi/causa-prima-scribo-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causa-prima/refs/heads/main/authentication/causa-prima-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Fintech
- E-Invoicing
- Invoicing
- Payments
- Compliance
- Germany
- EN 16931
- Agents
- MCP
---
