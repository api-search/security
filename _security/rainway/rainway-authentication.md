---
api_key_in: []
api_specs:
- filename: rainway-hub-api-openapi.yml
  format: yaml
  label: Rainway Hub API
  slug: rainway-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainway/refs/heads/main/openapi/rainway-hub-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rainway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rainway
provider_slug: rainway
scheme_count: 1
schemes:
- description: HTTP Basic authentication using a Rainway API Key Pair — username is the public key (pk_live_...), password is the secret key (sk_live_...).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/rainway-hub-api-openapi.yml
  type: http
slug: rainway-authentication
source_filename: rainway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/rainway-hub-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a Rainway API Key Pair — username is the public\n    key (pk_live_...), password is the secret key (sk_live_...).\n  sources:\n  - openapi/rainway-hub-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainway/refs/heads/main/authentication/rainway-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Streaming
- Application Streaming
- WebRTC
- Game Streaming
- SDK
- Real-Time
- Developer Platform
---
