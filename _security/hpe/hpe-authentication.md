---
api_key_in: []
api_specs:
- filename: hpe-openapi.yml
  format: yaml
  label: HPE GreenLake API
  slug: greenlake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hpe/refs/heads/main/openapi/hpe-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hpe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hewlett Packard Enterprise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hewlett Packard Enterprise
provider_slug: hpe
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 client-credentials access token. Use the token as

    `Authorization: Bearer <token>` on every request.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hpe-openapi.yml
  type: http
slug: hpe-authentication
source_filename: hpe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hpe-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 client-credentials access token. Use the token as\n    `Authorization: Bearer <token>` on every request.\n  sources:\n  - openapi/hpe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hpe/refs/heads/main/authentication/hpe-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Edge to Cloud
- Infrastructure as a Service
- Compute
- Storage
- Networking
- Hybrid Cloud
- Enterprise IT
---
