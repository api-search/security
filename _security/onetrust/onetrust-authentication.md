---
api_key_in: []
api_specs:
- filename: onetrust-openapi.yml
  format: yaml
  label: OneTrust Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/openapi/onetrust-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Onetrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneTrust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OneTrust
provider_slug: onetrust
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token issued via OAuth 2.0 client credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/onetrust-openapi.yml
  type: http
slug: onetrust-authentication
source_filename: onetrust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/onetrust-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token issued via OAuth 2.0 client credentials.\n  sources:\n  - openapi/onetrust-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetrust/refs/heads/main/authentication/onetrust-authentication.yml
summary_line: http · 1 scheme
tags:
- Privacy
- GRC
- Compliance
- Consent
- TPRM
---
