---
api_key_in: []
api_specs:
- filename: sysaid-openapi.yml
  format: yaml
  label: SysAid REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sysaid Authentication
name_suffix: Authentication
oauth_flows: []
overview: SysAid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SysAid
provider_slug: sysaid
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant: exchange client_id and client_secret at /generateaccesstoken for a short-lived access token (default 24h), then pass as "Authorization: Bearer <token>".'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sysaid-openapi.yml
  type: http
slug: sysaid-authentication
source_filename: sysaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sysaid-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 Client Credentials grant: exchange client_id and client_secret at\n    /generateaccesstoken for a short-lived access token (default 24h), then pass as \"Authorization:\n    Bearer <token>\".'\n  sources:\n  - openapi/sysaid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/authentication/sysaid-authentication.yml
summary_line: http · 1 scheme
tags:
- ITSM
- Help Desk
- IT Service Management
- Asset Management
- Ticketing
- Service Desk
---
