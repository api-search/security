---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hasfiyat-fiyatlar-api-openapi.yml
  format: yaml
  label: Hasfiyat Fiyatlar API
  slug: hasfiyat-fiyatlar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasfiyat/refs/heads/main/openapi/hasfiyat-fiyatlar-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Hasfiyat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hasfiyat secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hasfiyat
provider_slug: hasfiyat
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <api-anahtari>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hasfiyat-openapi.json
  type: http
- description: 'x-api-key: <api-anahtari>'
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/hasfiyat-openapi.json
  type: apiKey
slug: hasfiyat-authentication
source_filename: hasfiyat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/hasfiyat-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <api-anahtari>'\n  sources:\n  - openapi/hasfiyat-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'x-api-key: <api-anahtari>'\n  sources:\n  - openapi/hasfiyat-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasfiyat/refs/heads/main/authentication/hasfiyat-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Jewelry
- Software
- Pricing
- Management
---
