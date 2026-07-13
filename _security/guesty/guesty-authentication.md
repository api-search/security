---
api_key_in: []
api_specs:
- filename: guesty-openapi.yml
  format: yaml
  label: Guesty Open API
  slug: guesty-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Guesty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guesty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Guesty
provider_slug: guesty
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/guesty-openapi.yml
  type: http
slug: guesty-authentication
source_filename: guesty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guesty-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/guesty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/authentication/guesty-authentication.yml
summary_line: http · 1 scheme
tags:
- Booking
- Hospitality
- Property Management
- Reservations
- Short-Term Rentals
- Vacation Rentals
---
