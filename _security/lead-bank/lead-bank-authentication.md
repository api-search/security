---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lead Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Bank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lead Bank
provider_slug: lead-bank
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lead-bank-openapi.json
  type: http
slug: lead-bank-authentication
source_filename: lead-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lead-bank-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lead-bank-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/authentication/lead-bank-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Sponsor Bank
- Embedded Finance
- Banking as a Service
- Payments
- Lending
- Cards
- Deposits
---
