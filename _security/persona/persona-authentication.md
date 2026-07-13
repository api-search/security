---
api_key_in: []
api_specs:
- filename: persona-openapi.yml
  format: yaml
  label: Persona API
  slug: persona
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/openapi/persona-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Persona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Persona secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Persona
provider_slug: persona
scheme_count: 1
schemes:
- description: 'Persona uses bearer-token authentication. Pass your API key as

    `Authorization: Bearer <YOUR_API_KEY>` on every request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/persona-openapi.yml
  type: http
slug: persona-authentication
source_filename: persona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/persona-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Persona uses bearer-token authentication. Pass your API key as\n    `Authorization: Bearer <YOUR_API_KEY>` on every request.\n  sources:\n  - openapi/persona-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persona/refs/heads/main/authentication/persona-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud Prevention
- Identity Verification
- KYC
---
