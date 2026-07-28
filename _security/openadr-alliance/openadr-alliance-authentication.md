---
api_key_in: []
api_specs:
- filename: openadr-3-1-1-openapi.yaml
  format: yaml
  label: OpenADR 3 API
  slug: openadr-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/openapi/openadr-3-1-1-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Openadr Alliance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: OpenADR Alliance secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: OpenADR Alliance
provider_slug: openadr-alliance
scheme_count: 2
schemes:
- description: Client credential flow.
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: auth/token
  name: oAuth2ClientCredentials
  sources:
  - openapi/openadr-3-0-0-openapi.yaml
  - openapi/openadr-3-0-1-openapi.yaml
  - openapi/openadr-3-1-0-openapi.yaml
  - openapi/openadr-3-1-1-openapi.yaml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openadr-3-0-0-openapi.yaml
  - openapi/openadr-3-0-1-openapi.yaml
  - openapi/openadr-3-1-0-openapi.yaml
  - openapi/openadr-3-1-1-openapi.yaml
  type: http
slug: openadr-alliance-authentication
source_filename: openadr-alliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/openadr-3-0-0-openapi.yaml, openapi/openadr-3-0-1-openapi.yaml, openapi/openadr-3-1-0-openapi.yaml,\n  openapi/openadr-3-1-1-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: auth/token\n    scopes: 6\n  description: Client credential flow.\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/authentication/openadr-alliance-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Demand Response
- Grid
- DER
- OpenADR
- Standards
- Smart Grid
- EV Charging
- Certification
---
