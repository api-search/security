---
api_key_in: []
api_specs:
- filename: at-protocol-openapi.yml
  format: yaml
  label: AT Protocol XRPC API
  slug: atproto-xrpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/openapi/at-protocol-openapi.yml
- filename: at-protocol-asyncapi.yml
  format: yaml
  label: AT Protocol Relay & Firehose
  slug: relay-firehose
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/asyncapi/at-protocol-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: At Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: AT Protocol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AT Protocol
provider_slug: at-protocol
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'AT Protocol XRPC bearer auth using the `accessJwt` returned by

    `com.atproto.server.createSession`. The `refreshJwt` is used for

    `com.atproto.server.refreshSession`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/at-protocol-openapi.yml
  type: http
slug: at-protocol-authentication
source_filename: at-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at-protocol-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    AT Protocol XRPC bearer auth using the `accessJwt` returned by\n    `com.atproto.server.createSession`. The `refreshJwt` is used for\n    `com.atproto.server.refreshSession`.\n  sources:\n  - openapi/at-protocol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-protocol/refs/heads/main/authentication/at-protocol-authentication.yml
summary_line: http · 1 scheme
tags:
- AT Protocol
- atproto
- Bluesky
- Federation
- Decentralized Social
- Social Networking
- DID
- Lexicon
- XRPC
- PDS
- Relay
- AppView
- Open Protocol
---
