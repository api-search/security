---
api_key_in: []
api_specs:
- filename: zendit-api.yml
  format: yaml
  label: Zendit API
  slug: zendit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendit/refs/heads/main/openapi/zendit-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zendit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zendit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zendit
provider_slug: zendit
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Bearer token authentication using your Zendit API key.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zendit-api.yml
  type: http
slug: zendit-authentication
source_filename: zendit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zendit-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Bearer token authentication using your Zendit API key.\n  sources:\n  - openapi/zendit-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendit/refs/heads/main/authentication/zendit-authentication.yml
summary_line: http · 1 scheme
tags:
- eSIM
- Gift Cards
- Mobile Top-Up
- Payments
- Prepaid
---
