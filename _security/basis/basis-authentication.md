---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Basis Enterprise API
  slug: basis-enterprise-api
  spec_type: OpenAPI
  url: https://api.basis.net/docs/
auth_types:
- http
- unknown
description: ''
kind: authentication
layout: security
method: derived
name: Basis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basis secures its APIs with http and unknown across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Basis
provider_slug: basis
scheme_count: 2
schemes:
- name: OAuth2
  sources:
  - openapi/basis-platform-api.json
  type: unknown
- name: Bearer
  scheme: bearer
  sources:
  - openapi/basis-platform-api.json
  type: http
slug: basis-authentication
source_filename: basis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basis-platform-api.json\nsummary:\n  types:\n  - http\n  - unknown\nschemes:\n- name: OAuth2\n  type: unknown\n  sources:\n  - openapi/basis-platform-api.json\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/basis-platform-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/authentication/basis-authentication.yml
summary_line: http/unknown · 2 schemes
tags:
- Programmatic Advertising
- DSP
- Media Buying
- Campaign Management
- Audience Targeting
- AdTech
---
