---
api_key_in: []
api_specs:
- filename: tratta-openapi.yml
  format: yaml
  label: Tratta API
  slug: tratta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/openapi/tratta-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tratta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tratta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tratta
provider_slug: tratta
scheme_count: 1
schemes:
- description: Bearer token provided by Tratta after organization setup
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tratta-openapi.yml
  type: http
slug: tratta-authentication
source_filename: tratta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tratta-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token provided by Tratta after organization setup\n  sources:\n  - openapi/tratta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tratta/refs/heads/main/authentication/tratta-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Collections
- Payments
- Debt Collection
- Fintech
---
