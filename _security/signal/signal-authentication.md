---
api_key_in: []
api_specs:
- filename: signal-server-openapi.yml
  format: yaml
  label: Signal Server
  slug: signal-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-server-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Signal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signal secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Signal
provider_slug: signal
scheme_count: 2
schemes:
- description: HTTP Basic authentication using the account UUID (or phone number) and password. The password is established during account registration.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/signal-server-openapi.yml
  type: http
- description: Bearer token authentication used for certain provisioning and registration flows.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/signal-server-openapi.yml
  type: http
slug: signal-authentication
source_filename: signal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signal-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the account UUID (or phone number) and password.\n    The password is established during account registration.\n  sources:\n  - openapi/signal-server-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication used for certain provisioning and registration flows.\n  sources:\n  - openapi/signal-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/authentication/signal-authentication.yml
summary_line: http · 2 schemes
tags:
- Encryption
- Messaging
- Security
- Cryptography
- Open Source
- Privacy
---
