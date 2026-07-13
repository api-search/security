---
api_key_in: []
api_specs:
- filename: emnify-api-openapi.yml
  format: yaml
  label: emnify REST API
  slug: emnify-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/openapi/emnify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Emnify Authentication
name_suffix: Authentication
oauth_flows: []
overview: emnify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: emnify
provider_slug: emnify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Retrieve a JWT via POST /api/v1/authenticate using an application_token or user credentials, then send it as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/emnify-api-openapi.yml
  type: http
slug: emnify-authentication
source_filename: emnify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emnify-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Retrieve a JWT via POST /api/v1/authenticate using an application_token or user\n    credentials, then send it as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/emnify-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emnify/refs/heads/main/authentication/emnify-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Internet of Things
- Cellular Connectivity
- IoT SIM
- eSIM
- Consumer eSIM
- SGP.32
- M2M
- NTN-IoT
- Satellite
- SuperNetwork
---
