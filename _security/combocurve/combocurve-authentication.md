---
api_key_in:
- header
api_specs:
- filename: combocurve-openapi.yml
  format: yaml
  label: ComboCurve REST API
  slug: combocurve-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/combocurve/refs/heads/main/openapi/combocurve-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Combocurve Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComboCurve secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ComboCurve
provider_slug: combocurve
scheme_count: 2
schemes:
- description: Company API key from the ComboCurve API & Sync page.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/combocurve-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Signed bearer token generated from the Service Account Key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/combocurve-openapi.yml
  type: http
slug: combocurve-authentication
source_filename: combocurve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/combocurve-openapi.yml\ndocs: https://docs.api.combocurve.com/api/getting-started\nflow:\n  style: dual-header\n  note: Every request requires BOTH an Authorization signed bearer token AND the x-api-key header.\n  credentials_source: https://yourcompany.combocurve.com/company/api-sync (CREATE & DOWNLOAD)\n  authorization: Signed JWT bearer token generated from the downloaded Service Account Key.\n  api_key: Company API key issued on the ComboCurve API & Sync page.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Company API key from the ComboCurve API & Sync page.\n  sources:\n  - openapi/combocurve-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Signed bearer token generated from the Service Account Key.\n  sources:\n  - openapi/combocurve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/combocurve/refs/heads/main/authentication/combocurve-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Vertical Software
- Oil and Gas
- Energy
- Forecasting
- Reserves
- Economics
- Upstream
- Petroleum Engineering
---
