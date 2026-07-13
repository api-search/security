---
api_key_in: []
api_specs:
- filename: hexa-openapi.yml
  format: yaml
  label: Hex API
  slug: hex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hexa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hex
provider_slug: hexa
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hexa-openapi.yml
  type: http
slug: hexa-authentication
source_filename: hexa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hexa-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hexa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/authentication/hexa-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Collaboration
- Data
- Notebooks
---
