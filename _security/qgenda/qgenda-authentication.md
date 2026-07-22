---
api_key_in: []
api_specs:
- filename: qgenda-openapi.yml
  format: yaml
  label: QGenda REST API
  slug: qgenda-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgenda/refs/heads/main/openapi/qgenda-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qgenda Authentication
name_suffix: Authentication
oauth_flows: []
overview: QGenda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QGenda
provider_slug: qgenda
scheme_count: 1
schemes:
- description: 'Access token returned by POST /v2/login. Send as Authorization: bearer <access_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qgenda-openapi.yml
  type: http
slug: qgenda-authentication
source_filename: qgenda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qgenda-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token returned by POST /v2/login. Send as Authorization: bearer <access_token>.'\n  sources:\n  - openapi/qgenda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qgenda/refs/heads/main/authentication/qgenda-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Scheduling
- Workforce Management
- Physician Scheduling
- On-Call
- Credentialing
- Clinical Operations
---
