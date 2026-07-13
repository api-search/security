---
api_key_in:
- header
api_specs:
- filename: tyk-gateway-api-openapi.yml
  format: yaml
  label: Tyk Gateway API
  slug: tyk-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-gateway-api-openapi.yml
- filename: tyk-dashboard-api-openapi.yml
  format: yaml
  label: Tyk Dashboard API
  slug: tyk-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-dashboard-api-openapi.yml
- filename: tyk-dashboard-admin-api-openapi.yml
  format: yaml
  label: Tyk Dashboard Admin API
  slug: tyk-dashboard-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-dashboard-admin-api-openapi.yml
- filename: tyk-mdcb-api-openapi.yml
  format: yaml
  label: Tyk MDCB API
  slug: tyk-mdcb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-mdcb-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tyk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tyk secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tyk
provider_slug: tyk
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Admin-Auth
  sources:
  - openapi/tyk-dashboard-admin-api-openapi.yml
  type: apiKey
- description: The Tyk Dashboard API Access Credentials
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tyk-dashboard-api-openapi.yml
  type: http
- description: Api key
  in: header
  name: api_key
  parameter: X-Tyk-Authorization
  sources:
  - openapi/tyk-gateway-api-openapi.yml
  - openapi/tyk-mdcb-api-openapi.yml
  type: apiKey
slug: tyk-authentication
source_filename: tyk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tyk-dashboard-admin-api-openapi.yml, openapi/tyk-dashboard-api-openapi.yml,\n  openapi/tyk-gateway-api-openapi.yml, openapi/tyk-mdcb-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Admin-Auth\n  sources:\n  - openapi/tyk-dashboard-admin-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The Tyk Dashboard API Access Credentials\n  sources:\n  - openapi/tyk-dashboard-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Tyk-Authorization\n  description: Api key\n  sources:\n  - openapi/tyk-gateway-api-openapi.yml\n  - openapi/tyk-mdcb-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/authentication/tyk-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
---
