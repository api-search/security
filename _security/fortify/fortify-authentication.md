---
api_key_in:
- header
api_specs:
- filename: v3
  format: yaml
  label: Fortify on Demand API
  slug: fortify-on-demand-api
  spec_type: OpenAPI
  url: https://api.ams.fortify.com/swagger/docs/v3
- filename: fortify-software-security-center-openapi.yml
  format: yaml
  label: Fortify Software Security Center API
  slug: fortify-software-security-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/openapi/fortify-software-security-center-openapi.yml
- filename: fortify-scancentral-dast-openapi.yml
  format: yaml
  label: Fortify ScanCentral DAST API
  slug: fortify-scancentral-dast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/openapi/fortify-scancentral-dast-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fortify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fortify secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fortify
provider_slug: fortify
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer token obtained from POST /oauth/token using either client_credentials or password grant type.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fortify-on-demand-openapi.yml
  type: http
- description: 'Fortify token-based authentication. Pass as: FORTIFYTOKEN <token_value>. Obtain a CI token from SSC Administration or use an SSC auth token.'
  in: header
  name: fortifyToken
  parameter: Authorization
  sources:
  - openapi/fortify-scancentral-dast-openapi.yml
  - openapi/fortify-software-security-center-openapi.yml
  type: apiKey
- description: HTTP Basic authentication. Only supported on the /tokens endpoint for obtaining API tokens.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fortify-software-security-center-openapi.yml
  type: http
slug: fortify-authentication
source_filename: fortify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fortify-on-demand-openapi.yml, openapi/fortify-scancentral-dast-openapi.yml,\n  openapi/fortify-software-security-center-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer token obtained from POST /oauth/token using either client_credentials\n    or password grant type.\n  sources:\n  - openapi/fortify-on-demand-openapi.yml\n- name: fortifyToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Fortify token-based authentication. Pass as: FORTIFYTOKEN <token_value>. Obtain\n    a CI token from SSC Administration or use an SSC auth token.'\n  sources:\n  - openapi/fortify-scancentral-dast-openapi.yml\n  - openapi/fortify-software-security-center-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Only\
  \ supported on the /tokens endpoint for obtaining\n    API tokens.\n  sources:\n  - openapi/fortify-software-security-center-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/authentication/fortify-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
---
