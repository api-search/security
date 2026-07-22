---
api_key_in: []
api_specs:
- filename: uncovr-api-openapi-original.json
  format: json
  label: Uncovr API
  slug: uncovr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncovr/refs/heads/main/openapi/uncovr-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uncovr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncovr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uncovr
provider_slug: uncovr
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/uncovr-api-openapi-original.json
  type: http
slug: uncovr-authentication
source_filename: uncovr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/uncovr-api-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/uncovr-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncovr/refs/heads/main/authentication/uncovr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Surgery
- Artificial Intelligence
- Computer Vision
- Medical Documentation
- Medical Billing
- Clinical Intelligence
---
