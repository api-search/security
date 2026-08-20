---
api_key_in: []
auth_types:
- sessionCredentials
description: ''
kind: authentication
layout: security
method: searched
name: Options Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Options Technology secures its APIs with sessionCredentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Options Technology
provider_slug: options-technology
scheme_count: 1
schemes:
- description: user + password passed to activOneApi.connect({ host, user, password }); session-scoped, entitlement-managed per data source.
  failure_codes:
  - invalidUser
  - invalidPassword
  - accessDenied
  - notLicensed
  name: activOneApiSession
  sources:
  - https://weboneapi.activfinancial.com/tutorials/
  - https://weboneapi.activfinancial.com/documentation/session/connect
  transport: wss (WebSocket, WebAssembly client)
  type: sessionCredentials
slug: options-technology-authentication
source_filename: options-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://weboneapi.activfinancial.com/tutorials/\nnotes: >-\n  No OpenAPI exists for this provider, so this profile is captured from the\n  published Web One API tutorials and reference rather than derived from\n  securitySchemes. Authentication is a username/password session login inside\n  the WebSocket connect handshake - activOneApi.connect({ host, user,\n  password }) - resolving to a Session on success and rejecting with a\n  StatusCode (invalidUser, invalidPassword, accessDenied, notLicensed) on\n  failure. Credentials are provisioned by sales (sales@options-it.com) and\n  governed by exchange entitlements; there is no self-serve signup, no API\n  keys, and no OAuth/OIDC surface (no /.well-known/openid-configuration or\n  oauth-authorization-server on any probed host).\nsummary:\n  types: [sessionCredentials]\n  self_serve: false\n  provisioning: sales / exchange entitlements\n  oauth2_flows: []\nschemes:\n- name: activOneApiSession\n\
  \  type: sessionCredentials\n  transport: wss (WebSocket, WebAssembly client)\n  description: user + password passed to activOneApi.connect({ host, user,\n    password }); session-scoped, entitlement-managed per data source.\n  failure_codes: [invalidUser, invalidPassword, accessDenied, notLicensed]\n  sources:\n  - https://weboneapi.activfinancial.com/tutorials/\n  - https://weboneapi.activfinancial.com/documentation/session/connect\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/options-technology/refs/heads/main/authentication/options-technology-authentication.yml
summary_line: sessionCredentials · 1 scheme
tags:
- Financial
- Market Data
- Real-Time
- Streaming
- Trading Infrastructure
- Exchange Data
- Managed Service
- Low Latency
---
