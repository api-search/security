---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: myhuiban-com-auth-api-openapi.yml
  format: yaml
  label: MyHuiban Auth API
  slug: myhuiban-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-auth-api-openapi.yml
- filename: myhuiban-com-conferences-api-openapi.yml
  format: yaml
  label: MyHuiban Conferences API
  slug: myhuiban-com-conferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-conferences-api-openapi.yml
- filename: myhuiban-com-journals-api-openapi.yml
  format: yaml
  label: MyHuiban Journals API
  slug: myhuiban-com-journals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-journals-api-openapi.yml
- filename: myhuiban-com-researchers-api-openapi.yml
  format: yaml
  label: MyHuiban Researchers API
  slug: myhuiban-com-researchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-researchers-api-openapi.yml
- filename: myhuiban-com-statistics-api-openapi.yml
  format: yaml
  label: MyHuiban Statistics API
  slug: myhuiban-com-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-statistics-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: MyHuiban Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyHuiban secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MyHuiban
provider_slug: myhuiban-com
scheme_count: 2
schemes:
- description: 'Free-account credential, either form: an API key created at https://www.myhuiban.com/account/api-keys (starts with `hb_`, never expires, revocable individually, metered per key — this is the one to use with MCP clients that only take a URL plus a fixed header), or a JWT issued by POST /api/login (valid ~6 months, not individually revocable). Send as `Authorization: Bearer <credential>`. All creden'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myhuiban-com-openapi.yml
  type: http
- description: Per-request x402 payment channel — PLANNED, NOT YET LIVE. The origin recognises this header once the edge injects it after verifying a payment, but the edge-side gateway is not enabled, so clients currently cannot pay per request. Use the anonymous tier or a free-account API key / JWT instead.
  in: header
  name: paidAccess
  parameter: X-Paid-Access
  sources:
  - openapi/myhuiban-com-openapi.yml
  type: apiKey
slug: myhuiban-com-authentication
source_filename: myhuiban-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myhuiban-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Free-account credential, either form: an API key created at https://www.myhuiban.com/account/api-keys\n    (starts with `hb_`, never expires, revocable individually, metered per key — this is the\n    one to use with MCP clients that only take a URL plus a fixed header), or a JWT issued by\n    POST /api/login (valid ~6 months, not individually revocable). Send as `Authorization: Bearer\n    <credential>`. All creden'\n  sources:\n  - openapi/myhuiban-com-openapi.yml\n- name: paidAccess\n  type: apiKey\n  in: header\n  parameter: X-Paid-Access\n  description: Per-request x402 payment channel — PLANNED, NOT YET LIVE. The origin recognises\n    this header once the edge injects it after verifying a payment, but the edge-side gateway\n    is not enabled,\
  \ so clients currently cannot pay per request. Use the anonymous tier or a\n    free-account API key / JWT instead.\n  sources:\n  - openapi/myhuiban-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/myhuiban-com/authentication/myhuiban-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Conferences
- Indexing
- Academic
- Data
---
