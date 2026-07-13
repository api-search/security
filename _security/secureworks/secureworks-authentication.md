---
api_key_in: []
api_specs:
- filename: secureworks-taegis-xdr-openapi.yml
  format: yaml
  label: Secureworks Taegis XDR API
  slug: secureworks-taegis-xdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secureworks/refs/heads/main/openapi/secureworks-taegis-xdr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Secureworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secureworks secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Secureworks
provider_slug: secureworks
scheme_count: 2
schemes:
- description: OAuth2 bearer access token from /auth/api/v2/auth/token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/secureworks-taegis-xdr-openapi.yml
  type: http
- description: HTTP Basic auth with client_id as username and client_secret as password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/secureworks-taegis-xdr-openapi.yml
  type: http
slug: secureworks-authentication
source_filename: secureworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/secureworks-taegis-xdr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer access token from /auth/api/v2/auth/token\n  sources:\n  - openapi/secureworks-taegis-xdr-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with client_id as username and client_secret as password\n  sources:\n  - openapi/secureworks-taegis-xdr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secureworks/refs/heads/main/authentication/secureworks-authentication.yml
summary_line: http · 2 schemes
tags:
- Cybersecurity
- XDR
- Threat Detection
- Security Operations
- Incident Response
- MDR
- Threat Intelligence
---
