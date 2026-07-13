---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kajabi Public API
  slug: kajabi-public-api
  spec_type: OpenAPI
  url: https://github.com/Kajabi/public_api_docs/blob/main/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kajabi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kajabi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kajabi
provider_slug: kajabi
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/kajabi-public-api-openapi.yml
  type: http
slug: kajabi-authentication
source_filename: kajabi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kajabi-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kajabi-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/authentication/kajabi-authentication.yml
summary_line: http · 1 scheme
tags:
- Creator Economy
- Online Courses
- Memberships
- E-Commerce
- Digital Products
- Contacts
- Webhooks
- Payments
---
