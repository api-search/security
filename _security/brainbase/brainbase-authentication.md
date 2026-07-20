---
api_key_in: []
api_specs:
- filename: brainbase-openapi-original.json
  format: json
  label: Brainbase API v1
  slug: brainbase-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/openapi/brainbase-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brainbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brainbase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brainbase
provider_slug: brainbase
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A short description for security scheme
  name: bearer
  scheme: bearer
  sources:
  - openapi/brainbase-openapi-original.json
  type: http
slug: brainbase-authentication
source_filename: brainbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brainbase-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A short description for security scheme\n  sources:\n  - openapi/brainbase-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/authentication/brainbase-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud
- Intellectual Property
- Brand Licensing
- Licensing Management
- Royalties
- Contracts
- Trademarks
- SaaS
---
