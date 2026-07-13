---
api_key_in: []
api_specs:
- filename: clearvin-openapi.yml
  format: yaml
  label: VIN Decode API
  slug: vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Vehicle History Report API
  slug: vehicle-history-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Report Preview API
  slug: report-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Account Authentication API
  slug: account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clearvin Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearVIN secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClearVIN
provider_slug: clearvin
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT obtained from /rest/vendor/login, sent as "Authorization: Bearer {token}". Tokens expire after 120 minutes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clearvin-openapi.yml
  type: http
slug: clearvin-authentication
source_filename: clearvin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clearvin-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT obtained from /rest/vendor/login, sent as \"Authorization: Bearer {token}\".\n    Tokens expire after 120 minutes.'\n  sources:\n  - openapi/clearvin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/authentication/clearvin-authentication.yml
summary_line: http · 1 scheme
tags:
- VIN
- Vehicle History
- Automotive
- NMVTIS
- Vehicle Data
---
