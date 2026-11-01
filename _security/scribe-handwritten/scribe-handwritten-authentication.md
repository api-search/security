---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scribe-handwritten-v0-endpoints-api-openapi.yml
  format: yaml
  label: Scribe Handwritten v0 Endpoints API
  slug: scribe-handwritten-v0-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-v0-endpoints-api-openapi.yml
- filename: scribe-handwritten-v1-endpoints-api-openapi.yml
  format: yaml
  label: Scribe Handwritten v1 Endpoints API
  slug: scribe-handwritten-v1-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-v1-endpoints-api-openapi.yml
- filename: scribe-handwritten-wallet-api-openapi.yml
  format: yaml
  label: Scribe Handwritten Wallet API
  slug: scribe-handwritten-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribe-handwritten/openapi/scribe-handwritten-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Scribe Handwritten Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scribe Handwritten secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scribe Handwritten
provider_slug: scribe-handwritten
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/scribe-handwritten-openapi.json
  type: http
slug: scribe-handwritten-authentication
source_filename: scribe-handwritten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/scribe-handwritten-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/scribe-handwritten-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/scribe-handwritten/authentication/scribe-handwritten-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Handwriting
- Digital
- Collaboration
- Productivity
---
