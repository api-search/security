---
api_key_in:
- header
api_specs:
- filename: qlik-sense-cloud-rest-api-openapi.yml
  format: yaml
  label: Qlik Cloud Platform REST API
  slug: qlik-cloud-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense/refs/heads/main/openapi/qlik-sense-cloud-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qlik Sense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qlik Sense secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qlik Sense
provider_slug: qlik-sense
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from the Qlik Cloud tenant. Use the /oauth/token endpoint or interactive login to obtain a token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qlik-sense-cloud-rest-api-openapi.yml
  type: http
- description: API key generated from the Qlik Cloud Management Console. Passed in the Authorization header as Bearer <api-key>.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/qlik-sense-cloud-rest-api-openapi.yml
  type: apiKey
slug: qlik-sense-authentication
source_filename: qlik-sense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qlik-sense-cloud-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from the Qlik Cloud tenant. Use the /oauth/token\n    endpoint or interactive login to obtain a token.\n  sources:\n  - openapi/qlik-sense-cloud-rest-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key generated from the Qlik Cloud Management Console. Passed in the Authorization\n    header as Bearer <api-key>.\n  sources:\n  - openapi/qlik-sense-cloud-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense/refs/heads/main/authentication/qlik-sense-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Business Intelligence
- Cloud
- Data Integration
- Visualization
---
