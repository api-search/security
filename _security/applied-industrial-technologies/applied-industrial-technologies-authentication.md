---
api_key_in: []
api_specs:
- filename: applied-industrial-technologies-openapi.yaml
  format: yaml
  label: Applied Industrial Technologies API
  slug: applied-industrial-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/openapi/applied-industrial-technologies-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Applied Industrial Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Applied Industrial Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Applied Industrial Technologies
provider_slug: applied-industrial-technologies
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/applied-industrial-technologies-openapi.yaml
  type: http
slug: applied-industrial-technologies-authentication
source_filename: applied-industrial-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/applied-industrial-technologies-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/applied-industrial-technologies-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/authentication/applied-industrial-technologies-authentication.yml
summary_line: http · 1 scheme
tags:
- Industrial Distribution
- Bearings
- Power Transmission
- Fluid Power
- Supply Chain
- Fortune 1000
---
