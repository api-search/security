---
api_key_in: []
api_specs:
- filename: lemonmarkets-brokerage-openapi.json
  format: json
  label: lemon.markets Brokerage API
  slug: brokerage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/openapi/lemonmarkets-brokerage-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemonmarkets Authentication
name_suffix: Authentication
oauth_flows: []
overview: lemon.markets secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: lemon.markets
provider_slug: lemonmarkets
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lemonmarkets-brokerage-openapi.json
  type: http
slug: lemonmarkets-authentication
source_filename: lemonmarkets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lemonmarkets-brokerage-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lemonmarkets-brokerage-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonmarkets/refs/heads/main/authentication/lemonmarkets-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Brokerage
- Investing
- Trading
- Embedded Finance
- Banking as a Service
- Securities
- Wealth Management
- Germany
- Europe
---
