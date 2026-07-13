---
api_key_in: []
api_specs:
- filename: etrade-openapi.yml
  format: yaml
  label: E*TRADE API
  slug: etrade
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etrade/refs/heads/main/openapi/etrade-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Etrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Etrade secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Etrade
provider_slug: etrade
scheme_count: 1
schemes:
- description: E*TRADE uses OAuth 1.0a. Obtain a request token, redirect the customer for authorization, exchange for an access token, then sign each request with HMAC-SHA1.
  name: oauth1
  scheme: OAuth
  sources:
  - openapi/etrade-openapi.yml
  type: http
slug: etrade-authentication
source_filename: etrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/etrade-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oauth1\n  type: http\n  scheme: OAuth\n  description: E*TRADE uses OAuth 1.0a. Obtain a request token, redirect the customer for authorization,\n    exchange for an access token, then sign each request with HMAC-SHA1.\n  sources:\n  - openapi/etrade-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etrade/refs/heads/main/authentication/etrade-authentication.yml
summary_line: http · 1 scheme
tags:
- Bonds
- Brokerage
- Financial
- Futures
- Options
- Stocks
- Trading
---
