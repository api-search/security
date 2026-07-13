---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Bitso Trading REST API (v3)
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.bitso.com/llms.txt
- filename: bitso-asyncapi.yml
  format: yaml
  label: Bitso WebSocket API
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitso/refs/heads/main/asyncapi/bitso-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bitso Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitso secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitso
provider_slug: bitso
scheme_count: 1
schemes:
- description: 'Bitso HMAC scheme. Send `Authorization: Bitso <key>:<nonce>:<signature>`

    where signature is `HMAC-SHA256(secret, nonce + method + path + body)`.'
  in: header
  name: bitsoAuth
  parameter: Authorization
  sources:
  - openapi/bitso-openapi.yml
  type: apiKey
slug: bitso-authentication
source_filename: bitso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitso-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bitsoAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Bitso HMAC scheme. Send `Authorization: Bitso <key>:<nonce>:<signature>`\n    where signature is `HMAC-SHA256(secret, nonce + method + path + body)`.\n  sources:\n  - openapi/bitso-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitso/refs/heads/main/authentication/bitso-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Trading
- Stablecoins
- Payouts
- Cross Border
- Latin America
- Mexico
- Fintech
---
