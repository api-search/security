---
api_key_in: []
api_specs:
- filename: platzi-fake-store-api-openapi.yml
  format: yaml
  label: Platzi Fake Store API
  slug: platzi-fake-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platzi-fake-store-api/refs/heads/main/openapi/platzi-fake-store-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Platzi Fake Store Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Platzi Fake Store API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Platzi Fake Store API
provider_slug: platzi-fake-store-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/platzi-fake-store-api-openapi.yml
  type: http
slug: platzi-fake-store-api-authentication
source_filename: platzi-fake-store-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/platzi-fake-store-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/platzi-fake-store-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platzi-fake-store-api/refs/heads/main/authentication/platzi-fake-store-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Fake API
- JWT
- Prototyping
- Sandbox
- Sample Data
- Testing
---
