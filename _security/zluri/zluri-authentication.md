---
api_key_in: []
api_specs:
- filename: zluri-api-openapi.yml
  format: yaml
  label: Zluri
  slug: zluri
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/openapi/zluri-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zluri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zluri secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zluri
provider_slug: zluri
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication. Obtain your API token from the Zluri admin dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zluri-api-openapi.yml
  type: http
slug: zluri-authentication
source_filename: zluri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zluri-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication. Obtain your API token from the Zluri admin dashboard.\n  sources:\n  - openapi/zluri-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/authentication/zluri-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- SaaS Management
---
