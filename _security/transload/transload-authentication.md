---
api_key_in: []
api_specs:
- filename: transload-pipeline-backend-openapi.json
  format: json
  label: Transload Pipeline Backend API
  slug: transload-pipeline-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transload/refs/heads/main/openapi/transload-pipeline-backend-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Transload Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transload secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Transload
provider_slug: transload
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/transload-pipeline-backend-openapi.json
  type: http
slug: transload-authentication
source_filename: transload-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/transload-pipeline-backend-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/transload-pipeline-backend-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transload/refs/heads/main/authentication/transload-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Freight
- Computer Vision
- Warehouses
- Supply Chain
- Measurement
- Cameras
- Trucking
---
