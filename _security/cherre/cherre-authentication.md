---
api_key_in: []
api_specs:
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Property API
  slug: property
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Tax Assessor API
  slug: tax-assessor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Recorder API
  slug: recorder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Owner & Parcel API
  slug: owner-parcel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
- filename: cherre-openapi.yml
  format: yaml
  label: Cherre Connections API
  slug: connections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/openapi/cherre-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cherre Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cherre secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cherre
provider_slug: cherre
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cherre-openapi.yml
  type: http
slug: cherre-authentication
source_filename: cherre-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cherre-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cherre-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cherre/refs/heads/main/authentication/cherre-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- Property Intelligence
- Data Integration
- Knowledge Graph
- GraphQL
---
