---
api_key_in: []
api_specs:
- filename: app-directory.html
  format: yaml
  label: FDC3 App Directory API
  slug: app-directory-api
  spec_type: OpenAPI
  url: https://fdc3.finos.org/schemas/2.2/app-directory.html
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fdc3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: FDC3 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FDC3
provider_slug: fdc3
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/app-directory-1.1.yaml
  - openapi/app-directory-1.2.yaml
  - openapi/app-directory-2.0.yaml
  - openapi/app-directory-2.1.json
  - openapi/app-directory-2.2.json
  type: http
slug: fdc3-authentication
source_filename: fdc3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/app-directory-1.1.yaml, openapi/app-directory-1.2.yaml, openapi/app-directory-2.0.yaml,\n  openapi/app-directory-2.1.json, openapi/app-directory-2.2.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/app-directory-1.1.yaml\n  - openapi/app-directory-1.2.yaml\n  - openapi/app-directory-2.0.yaml\n  - openapi/app-directory-2.1.json\n  - openapi/app-directory-2.2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdc3/refs/heads/main/authentication/fdc3-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Services
- Fintech
- Desktop Interoperability
- Open Standard
- FINOS
- Context Sharing
- Intents
---
