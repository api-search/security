---
api_key_in: []
api_specs:
- filename: nabla-openapi.yml
  format: yaml
  label: Nabla Core API
  slug: nabla-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabla/refs/heads/main/openapi/nabla-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nabla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nabla secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nabla
provider_slug: nabla
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token (Server API) or JWT access token (User API).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nabla-openapi.yml
  type: http
slug: nabla-authentication
source_filename: nabla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nabla-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token (Server API) or JWT access token (User API).\n  sources:\n  - openapi/nabla-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabla/refs/heads/main/authentication/nabla-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Ambient AI
- Clinical Documentation
- Medical Transcription
- Speech Recognition
- FHIR
- SOAP Notes
- Voice
- EHR Integration
---
