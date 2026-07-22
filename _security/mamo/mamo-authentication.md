---
api_key_in: []
api_specs:
- filename: mamo-openapi.yml
  format: yaml
  label: Mamo Business API
  slug: mamo-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mamo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mamo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mamo
provider_slug: mamo
scheme_count: 1
schemes:
- description: 'API key from the Mamo dashboard (Developer > Keys), passed as `Authorization: Bearer <api_key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mamo-openapi.yml
  type: http
slug: mamo-authentication
source_filename: mamo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mamo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from the Mamo dashboard (Developer > Keys), passed as `Authorization:\n    Bearer <api_key>`.'\n  sources:\n  - openapi/mamo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/authentication/mamo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Fintech
- Payment Links
- Subscriptions
- Corporate Cards
- Payouts
- Expense Management
- UAE
- Middle East
---
