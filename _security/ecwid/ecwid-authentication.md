---
api_key_in: []
api_specs:
- filename: ecwid-openapi.yml
  format: yaml
  label: Ecwid REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ecwid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ecwid by Lightspeed secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ecwid by Lightspeed
provider_slug: ecwid
scheme_count: 1
schemes:
- description: OAuth 2.0 access token (private or public) used as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ecwid-openapi.yml
  type: http
slug: ecwid-authentication
source_filename: ecwid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ecwid-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token (private or public) used as a Bearer token.\n  sources:\n  - openapi/ecwid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/authentication/ecwid-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Online Store
- Storefront
- Retail
- Point of Sale
- Multi-Channel Commerce
---
