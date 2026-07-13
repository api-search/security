---
api_key_in: []
api_specs:
- filename: port-io-openapi.yml
  format: yaml
  label: Port REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-io/refs/heads/main/openapi/port-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Port Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Port secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Port
provider_slug: port-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Port uses bearer tokens obtained from the Port application credentials panel.

    Tokens remain valid for 3 hours.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/port-io-openapi.yml
  type: http
slug: port-io-authentication
source_filename: port-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/port-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Port uses bearer tokens obtained from the Port application credentials panel.\n    Tokens remain valid for 3 hours.\n  sources:\n  - openapi/port-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port-io/refs/heads/main/authentication/port-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Internal Developer Portal
- Service Catalog
- Self-Service Actions
- Platform Engineering
- Scorecards
- Developer Experience
---
