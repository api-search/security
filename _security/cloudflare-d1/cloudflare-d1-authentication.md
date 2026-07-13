---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare D1 API
  slug: cloudflare-d1-api
  spec_type: OpenAPI
  url: https://developers.cloudflare.com/api/resources/d1/subresources/database/
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudflare D1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudflare D1 secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloudflare D1
provider_slug: cloudflare-d1
scheme_count: 4
schemes:
- in: header
  name: api_email
  parameter: X-Auth-Email
  sources:
  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: X-Auth-Key
  sources:
  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml
  type: apiKey
- name: api_token
  scheme: bearer
  sources:
  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml
  type: http
- in: header
  name: user_service_key
  parameter: X-Auth-User-Service-Key
  sources:
  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml
  type: apiKey
slug: cloudflare-d1-authentication
source_filename: cloudflare-d1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_email\n  type: apiKey\n  in: header\n  parameter: X-Auth-Email\n  sources:\n  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  sources:\n  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\n- name: api_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\n- name: user_service_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-User-Service-Key\n  sources:\n  - openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-d1/refs/heads/main/authentication/cloudflare-d1-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Database
- SQLite
- Serverless
- Edge Computing
- SQL
- Cloudflare
- Workers
---
