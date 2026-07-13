---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Dryad REST API
  slug: dryad-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dryad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dryad secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dryad
provider_slug: dryad
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: dryad-authentication
source_filename: dryad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/authentication/dryad-authentication.yml
summary_line: http · 1 scheme
tags:
- Research Data
- Open Science
- Data Repository
- Datasets
- Biology
- Ecology
- Open Access
---
