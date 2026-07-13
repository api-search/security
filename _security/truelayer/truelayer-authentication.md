---
api_key_in: []
api_specs:
- filename: truelayer-payments-openapi.yml
  format: yaml
  label: TrueLayer Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truelayer/refs/heads/main/openapi/truelayer-payments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Truelayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueLayer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueLayer
provider_slug: truelayer
scheme_count: 1
schemes:
- description: OAuth2 access token with payments scope
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/truelayer-payments-openapi.yml
  type: http
slug: truelayer-authentication
source_filename: truelayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truelayer-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 access token with payments scope\n  sources:\n  - openapi/truelayer-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truelayer/refs/heads/main/authentication/truelayer-authentication.yml
summary_line: http · 1 scheme
tags:
- Data API
- Financial Services
- Open Banking
- Payments
- PSD2
- UK Banking
- VRP
---
