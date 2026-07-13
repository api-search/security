---
api_key_in: []
api_specs:
- filename: fashn-openapi.yml
  format: yaml
  label: FASHN
  slug: fashn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fashn/refs/heads/main/openapi/fashn-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fashn Authentication
name_suffix: Authentication
oauth_flows: []
overview: FASHN AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FASHN AI
provider_slug: fashn
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fashn-openapi.yml
  type: http
slug: fashn-authentication
source_filename: fashn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fashn-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/fashn-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashn/refs/heads/main/authentication/fashn-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Clothing
- Fashion
- Virtual Try-On
---
