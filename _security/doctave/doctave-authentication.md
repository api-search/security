---
api_key_in: []
api_specs:
- filename: doctave-doctave-openapi.yml
  format: yaml
  label: Doctave API
  slug: doctave
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/openapi/doctave-doctave-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doctave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doctave secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doctave
provider_slug: doctave
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Authentication token obtained from the Doctave dashboard or via API key management.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/doctave-doctave-openapi.yml
  type: http
slug: doctave-authentication
source_filename: doctave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doctave-doctave-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Authentication token obtained from the Doctave dashboard or via API key management.\n  sources:\n  - openapi/doctave-doctave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/authentication/doctave-authentication.yml
summary_line: http · 1 scheme
tags:
- Documentation
- OpenAPI
- Platform
- Portals
---
