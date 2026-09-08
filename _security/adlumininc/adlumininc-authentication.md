---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adlumininc-api-openapi-original.yml
  format: yaml
  label: Adlumin XDR/MDR API
  slug: adlumin-xdrmdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adlumininc/refs/heads/main/openapi/adlumininc-api-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adlumininc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adlumin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adlumin
provider_slug: adlumininc
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT issued by the Adlumin authentication service. Pass in the Authorization header as `Bearer <token>`.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/adlumininc-api-openapi-original.yml
  type: http
slug: adlumininc-authentication
source_filename: adlumininc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/adlumininc-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT issued by the Adlumin authentication service. Pass in the Authorization header\n    as `Bearer <token>`.\n  sources:\n  - openapi/adlumininc-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adlumininc/refs/heads/main/authentication/adlumininc-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Cybersecurity
- Managed Detection and Response
- Extended Detection and Response
- SIEM
- SOAR
- Threat Detection
- Endpoint Security
- Compliance
- Managed Service Providers
- MCP
- agent-native
---
