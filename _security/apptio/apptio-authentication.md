---
api_key_in: []
api_specs:
- filename: apptio-openapi.yaml
  format: yaml
  label: Apptio API
  slug: apptio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptio/refs/heads/main/openapi/apptio-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apptio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apptio
provider_slug: apptio
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apptio-openapi.yaml
  type: http
slug: apptio-authentication
source_filename: apptio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apptio-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/apptio-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptio/refs/heads/main/authentication/apptio-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Cost Management
- IT Finance
- Technology Business Management
---
