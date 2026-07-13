---
api_key_in: []
api_specs:
- filename: frp-server-admin-api-openapi.yml
  format: yaml
  label: frp Server Admin API
  slug: server-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/openapi/frp-server-admin-api-openapi.yml
- filename: frp-client-admin-api-openapi.yml
  format: yaml
  label: frp Client Admin API
  slug: client-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/openapi/frp-client-admin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Frp Authentication
name_suffix: Authentication
oauth_flows: []
overview: frp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: frp
provider_slug: frp
scheme_count: 1
schemes:
- description: HTTP Basic auth using webServer.user and webServer.password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/frp-client-admin-api-openapi.yml
  - openapi/frp-server-admin-api-openapi.yml
  type: http
slug: frp-authentication
source_filename: frp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/frp-client-admin-api-openapi.yml, openapi/frp-server-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using webServer.user and webServer.password\n  sources:\n  - openapi/frp-client-admin-api-openapi.yml\n  - openapi/frp-server-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/authentication/frp-authentication.yml
summary_line: http · 1 scheme
tags:
- NAT Traversal
- Reverse Proxy
- Tunneling
- Open Source
---
