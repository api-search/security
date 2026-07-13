---
api_key_in: []
api_specs:
- filename: bloomberg-data-license-api.yml
  format: yaml
  label: Bloomberg Data License API
  slug: bloomberg-data-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-data-license-api.yml
- filename: bloomberg-emsx-api.yml
  format: yaml
  label: Bloomberg EMSX API
  slug: bloomberg-emsx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-emsx-api.yml
- filename: bloomberg-http-api.yml
  format: yaml
  label: Bloomberg HTTP API
  slug: bloomberg-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-http-api.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bloomberg Aim Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bloomberg AIM secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Bloomberg-issued JWT credential obtained from the Bloomberg Console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bloomberg-data-license-api.yml
  - openapi/bloomberg-emsx-api.yml
  type: http
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2
  name: oauth2
  sources:
  - openapi/bloomberg-data-license-api.yml
  type: oauth2
- description: HTTP Basic authentication for the local API server
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bloomberg-http-api.yml
  type: http
slug: bloomberg-aim-authentication
source_filename: bloomberg-aim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-data-license-api.yml, openapi/bloomberg-emsx-api.yml, openapi/bloomberg-http-api.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bloomberg-issued JWT credential obtained from the Bloomberg Console.\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n  - openapi/bloomberg-emsx-api.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2\n    scopes: 3\n  description: OAuth 2.0 client credentials flow\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication for the local API server\n  sources:\n  - openapi/bloomberg-http-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/authentication/bloomberg-aim-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
---
