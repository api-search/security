---
api_key_in: []
api_specs:
- filename: embat-openapi-original.json
  format: json
  label: Embat API
  slug: embat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/embat/refs/heads/main/openapi/embat-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Embat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Embat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Embat
provider_slug: embat
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/embat-openapi-original.json
  type: http
slug: embat-authentication
source_filename: embat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/embat-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/embat-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embat/refs/heads/main/authentication/embat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Treasury Management
- Payments
- Cash Flow
- Banking
- Reconciliation
- Forecasting
---
