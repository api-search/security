---
api_key_in: []
api_specs:
- filename: sabre-bargain-finder-max-openapi.yml
  format: yaml
  label: Sabre Bargain Finder Max API
  slug: bargain-finder-max
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/openapi/sabre-bargain-finder-max-openapi.yml
- filename: sabre-hotels-openapi.yml
  format: yaml
  label: Sabre Hotels API
  slug: hotels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/openapi/sabre-hotels-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sabre Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sabre secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sabre
provider_slug: sabre
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from /v2/auth/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sabre-bargain-finder-max-openapi.yml
  - openapi/sabre-hotels-openapi.yml
  type: http
slug: sabre-authentication
source_filename: sabre-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sabre-bargain-finder-max-openapi.yml, openapi/sabre-hotels-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from /v2/auth/token\n  sources:\n  - openapi/sabre-bargain-finder-max-openapi.yml\n  - openapi/sabre-hotels-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/authentication/sabre-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- GDS
- Airlines
- Hotels
- Car Rental
- Booking
---
