---
api_key_in:
- cookie
- header
api_specs:
- filename: netcracker-qubership-apihub-registry-openapi.yml
  format: yaml
  label: Qubership APIHUB Registry API
  slug: qubership-apihub-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-registry-openapi.yml
- filename: netcracker-qubership-apihub-admin-openapi.yml
  format: yaml
  label: Qubership APIHUB System Administrators API
  slug: qubership-apihub-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-admin-openapi.yml
- filename: netcracker-qubership-maas-swagger.yml
  format: yaml
  label: Qubership MaaS (Messaging as a Service) API
  slug: qubership-maas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-maas-swagger.yml
- filename: netcracker-qubership-dbaas-openapi.json
  format: json
  label: Qubership DBaaS Aggregator API
  slug: qubership-dbaas-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-dbaas-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Netcracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netcracker secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Netcracker
provider_slug: netcracker
scheme_count: 6
schemes:
- bearerFormat: JWT
  description: 'Bearer token authentication (JWT). Default security scheme for API usage. Provide Authorization: Bearer <token>.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/netcracker-qubership-apihub-admin-openapi.yml
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  - openapi/netcracker-qubership-dbaas-openapi.json
  type: http
- description: Authentication via the `apihub-access-token` cookie.
  in: cookie
  name: CookieAuth
  parameter: apihub-access-token
  sources:
  - openapi/netcracker-qubership-apihub-admin-openapi.yml
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  type: apiKey
- description: API key authentication. Send the key in the api-key header.
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/netcracker-qubership-apihub-admin-openapi.yml
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  type: apiKey
- description: Personal access token authentication. Send the token in the X-Personal-Access-Token header; use for user-issued/script access.
  in: header
  name: PersonalAccessToken
  parameter: X-Personal-Access-Token
  sources:
  - openapi/netcracker-qubership-apihub-admin-openapi.yml
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  type: apiKey
- description: Authentication via refresh token cookie
  in: cookie
  name: RefreshTokenAuth
  parameter: apihub-refresh-token
  sources:
  - openapi/netcracker-qubership-apihub-admin-openapi.yml
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  type: apiKey
- description: Login/password authentication.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/netcracker-qubership-apihub-registry-openapi.yml
  - openapi/netcracker-qubership-maas-swagger.yml
  type: http
slug: netcracker-authentication
source_filename: netcracker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/netcracker-qubership-apihub-admin-openapi.yml, openapi/netcracker-qubership-apihub-registry-openapi.yml,\n  openapi/netcracker-qubership-dbaas-openapi.json, openapi/netcracker-qubership-maas-swagger.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Bearer token authentication (JWT). Default security scheme for API usage. Provide\n    Authorization: Bearer <token>.'\n  sources:\n  - openapi/netcracker-qubership-apihub-admin-openapi.yml\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n  - openapi/netcracker-qubership-dbaas-openapi.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: apihub-access-token\n  description: Authentication via the `apihub-access-token` cookie.\n  sources:\n  - openapi/netcracker-qubership-apihub-admin-openapi.yml\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n\
  - name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key authentication. Send the key in the api-key header.\n  sources:\n  - openapi/netcracker-qubership-apihub-admin-openapi.yml\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n- name: PersonalAccessToken\n  type: apiKey\n  in: header\n  parameter: X-Personal-Access-Token\n  description: Personal access token authentication. Send the token in the X-Personal-Access-Token\n    header; use for user-issued/script access.\n  sources:\n  - openapi/netcracker-qubership-apihub-admin-openapi.yml\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n- name: RefreshTokenAuth\n  type: apiKey\n  in: cookie\n  parameter: apihub-refresh-token\n  description: Authentication via refresh token cookie\n  sources:\n  - openapi/netcracker-qubership-apihub-admin-openapi.yml\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description:\
  \ Login/password authentication.\n  sources:\n  - openapi/netcracker-qubership-apihub-registry-openapi.yml\n  - openapi/netcracker-qubership-maas-swagger.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/authentication/netcracker-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Telecommunications
- United States
- BSS
- OSS
- Network Vendor
- API Management
- TM Forum
- Open API
- CAMARA
- Standards
- Orchestration
- Monetization
- Open Source
---
