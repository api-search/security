---
api_key_in: []
api_specs:
- filename: aruba-central-api.yml
  format: yaml
  label: Aruba Central API
  slug: aruba-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/openapi/aruba-central-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aruba Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aruba secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aruba
provider_slug: aruba
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained through the Aruba Central API Gateway three-step OAuth flow. Tokens expire after 7200 seconds (2 hours) and can be refreshed using the refresh_token grant type.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aruba-central-api.yml
  type: http
slug: aruba-authentication
source_filename: aruba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aruba-central-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained through the Aruba Central API Gateway three-step\n    OAuth flow. Tokens expire after 7200 seconds (2 hours) and can be refreshed using the refresh_token\n    grant type.\n  sources:\n  - openapi/aruba-central-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/authentication/aruba-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
---
