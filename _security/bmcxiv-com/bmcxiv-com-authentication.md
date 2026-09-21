---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bmcxiv-com-openapi.yml
  format: yaml
  label: Breach402 API
  slug: breach402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmcxiv-com/refs/heads/main/openapi/bmcxiv-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bmcxiv Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BMC XIV secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BMC XIV
provider_slug: bmcxiv-com
scheme_count: 1
schemes:
- bearerFormat: opaque-token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bmcxiv-com-openapi.yml
  type: http
slug: bmcxiv-com-authentication
source_filename: bmcxiv-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/bmcxiv-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque-token\n  sources:\n  - openapi/bmcxiv-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmcxiv-com/refs/heads/main/authentication/bmcxiv-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Breach Intelligence
- Identity Protection
- Data Breaches
- Agents
- MCP
- A2A
- x402
---
