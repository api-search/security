---
api_key_in: []
api_specs:
- filename: opera-inventory-api-openapi.yml
  format: yaml
  label: Opera Inventory API
  slug: opera-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-inventory-api-openapi.yml
- filename: opera-marketing-api-openapi.yml
  format: yaml
  label: Opera Marketing API
  slug: opera-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-marketing-api-openapi.yml
- filename: opera-report-api-openapi.yml
  format: yaml
  label: Opera Report API
  slug: opera-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/openapi/opera-report-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opera
provider_slug: opera
scheme_count: 1
schemes:
- description: 'API token issued by Opera Ads, passed as `Authorization: Bearer <token>`. Contact Opera Ads to obtain credentials.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opera-ads-openapi.yml
  type: http
slug: opera-authentication
source_filename: opera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opera-ads-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued by Opera Ads, passed as `Authorization: Bearer <token>`. Contact\n    Opera Ads to obtain credentials.'\n  sources:\n  - openapi/opera-ads-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opera/refs/heads/main/authentication/opera-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer Technology
- Advertising
- AdTech
- Browser
- Monetization
- OpenRTB
- Marketing
---
