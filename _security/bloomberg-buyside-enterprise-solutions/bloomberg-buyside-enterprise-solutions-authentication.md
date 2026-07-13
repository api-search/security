---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bloomberg Buyside Enterprise Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg Buyside Enterprise Solutions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bloomberg API bearer token obtained via OAuth 2.0 authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bloomberg-buyside-analytics-openapi.yml
  - openapi/bloomberg-buyside-data-openapi.yml
  - openapi/bloomberg-buyside-order-management-openapi.yml
  - openapi/bloomberg-buyside-portfolio-openapi.yml
  type: http
slug: bloomberg-buyside-enterprise-solutions-authentication
source_filename: bloomberg-buyside-enterprise-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-buyside-analytics-openapi.yml, openapi/bloomberg-buyside-data-openapi.yml,\n  openapi/bloomberg-buyside-order-management-openapi.yml, openapi/bloomberg-buyside-portfolio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bloomberg API bearer token obtained via OAuth 2.0 authentication\n  sources:\n  - openapi/bloomberg-buyside-analytics-openapi.yml\n  - openapi/bloomberg-buyside-data-openapi.yml\n  - openapi/bloomberg-buyside-order-management-openapi.yml\n  - openapi/bloomberg-buyside-portfolio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-buyside-enterprise-solutions/refs/heads/main/authentication/bloomberg-buyside-enterprise-solutions-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
---
