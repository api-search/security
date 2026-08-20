---
api_key_in: []
api_specs:
- filename: circle-pharma-content-openapi.yml
  format: yaml
  label: Circle Pharma Content API
  slug: circle-pharma-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circle Pharma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle Pharma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circle Pharma
provider_slug: circle-pharma
scheme_count: 1
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for write and administrative routes, which are out of scope for this document — every operation modelled here is anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/circle-pharma-content-openapi.yml
  type: http
slug: circle-pharma-authentication
source_filename: circle-pharma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/circle-pharma-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for\n    write and administrative routes, which are out of scope for this document — every operation\n    modelled here is anonymous.\n  sources:\n  - openapi/circle-pharma-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/authentication/circle-pharma-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Drug Discovery
- Macrocycles
- Clinical Trials
- Life Sciences
- content-api
---
