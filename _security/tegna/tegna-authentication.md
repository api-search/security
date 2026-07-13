---
api_key_in:
- header
api_specs:
- filename: tegna-audience-one-openapi.yml
  format: yaml
  label: TEGNA AudienceOne API
  slug: audience-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-audience-one-openapi.yml
- filename: tegna-premion-openapi.yml
  format: yaml
  label: TEGNA Premion OTT Advertising API
  slug: premion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-premion-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tegna Authentication
name_suffix: Authentication
oauth_flows: []
overview: TEGNA secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TEGNA
provider_slug: tegna
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tegna-audience-one-openapi.yml
  type: http
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tegna-premion-openapi.yml
  type: apiKey
slug: tegna-authentication
source_filename: tegna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tegna-audience-one-openapi.yml, openapi/tegna-premion-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/tegna-audience-one-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/tegna-premion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/authentication/tegna-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Broadcasting
- Media
- Television
- Digital Advertising
- OTT
- CTV
- Fortune 500
---
