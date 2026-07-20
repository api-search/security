---
api_key_in: []
api_specs:
- filename: brellium-openapi-original.json
  format: json
  label: Brellium API
  slug: brellium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brellium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brellium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brellium
provider_slug: brellium
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/brellium-openapi-original.json
  type: http
slug: brellium-authentication
source_filename: brellium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brellium-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/brellium-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/authentication/brellium-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Clinical Compliance
- Clinical Documentation
- Medical Coding
- Audit
- Behavioral Health
- Digital Health
- API
---
