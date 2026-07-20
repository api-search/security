---
api_key_in: []
api_specs:
- filename: laurel-time-openapi-original.json
  format: json
  label: Laurel Time Service API
  slug: time
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-time-openapi-original.json
- filename: laurel-identity-openapi-original.json
  format: json
  label: Laurel Identity Service API
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-identity-openapi-original.json
- filename: laurel-ingestion-openapi-original.json
  format: json
  label: Laurel Ingestion Service API
  slug: ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-ingestion-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Laurel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laurel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Laurel
provider_slug: laurel
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter access token
  name: ApiBearerAuth
  scheme: bearer
  sources:
  - openapi/laurel-identity-openapi-original.json
  - openapi/laurel-ingestion-openapi-original.json
  - openapi/laurel-time-openapi-original.json
  type: http
slug: laurel-authentication
source_filename: laurel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/laurel-identity-openapi-original.json, openapi/laurel-ingestion-openapi-original.json,\n  openapi/laurel-time-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter access token\n  sources:\n  - openapi/laurel-identity-openapi-original.json\n  - openapi/laurel-ingestion-openapi-original.json\n  - openapi/laurel-time-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/authentication/laurel-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Timekeeping
- Time Tracking
- Legal
- Legal Tech
- Accounting
- Professional Services
- Billing
- Practice Management
- Work Intelligence
- Analytics
---
