---
api_key_in: []
api_specs:
- filename: amtrust-financial-services-commercial-lines-api.yaml
  format: yaml
  label: AmTrust Commercial Lines API
  slug: commercial-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-commercial-lines-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amtrust Financial Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: AmTrust Financial Services secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from /oauth/token endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/amtrust-financial-services-commercial-lines-api.yaml
  type: http
slug: amtrust-financial-services-authentication
source_filename: amtrust-financial-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amtrust-financial-services-commercial-lines-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from /oauth/token endpoint\n  sources:\n  - openapi/amtrust-financial-services-commercial-lines-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/authentication/amtrust-financial-services-authentication.yml
summary_line: http · 1 scheme
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
- Fortune 1000
---
