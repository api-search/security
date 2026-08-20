---
api_key_in: []
auth_types:
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Doodles Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doodles secures its APIs with hmac-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doodles
provider_slug: doodles
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  direction: inbound-to-your-receiver
  encoding: base64
  in: header
  key_material: shared secret provisioned out of band
  name: webhookSignature
  parameter_name: x-signature
  signed_material: raw JSON request body
  sources:
  - https://github.com/Doodles/webhook-example
  type: hmac
  verification: constant-time compare; reject with HTTP 403 on mismatch
slug: doodles-authentication
source_filename: doodles-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://github.com/Doodles/webhook-example\ndocs: https://github.com/Doodles/webhook-example#signature-verification\nscope: >-\n  Covers the ONLY authenticated integration surface Doodles publishes — the outbound\n  webhook contract. Doodles operates no public REST API, issues no API keys, and runs\n  no OAuth 2.0 / OpenID Connect authorization server that could be discovered\n  anonymously; /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server were probed on www.doodles.app and\n  stoodio.doodles.app and both hosts answered a 429 bot challenge rather than a\n  document (see well-known/doodles-well-known.yml).\nsummary:\n  types: [hmac-signature]\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  mutual_tls: false\nschemes:\n- name: webhookSignature\n  type: hmac\n  algorithm: HMAC-SHA256\n  encoding: base64\n  in: header\n  parameter_name: x-signature\n  signed_material: raw JSON request body\n\
  \  key_material: shared secret provisioned out of band\n  direction: inbound-to-your-receiver\n  verification: constant-time compare; reject with HTTP 403 on mismatch\n  sources: [https://github.com/Doodles/webhook-example]\nnot_found:\n- {mechanism: apiKey, note: No public API key program or developer console was discoverable.}\n- {mechanism: oauth2, note: No authorization/token endpoints published.}\n- {mechanism: openIdConnect, note: /.well-known/openid-configuration answered 429 (bot challenge), not a document.}\n- {mechanism: mutualTLS, note: Not documented.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doodles/refs/heads/main/authentication/doodles-authentication.yml
summary_line: hmac-signature · 1 scheme
tags:
- Company
- NFT
- Web3
- Blockchain
- Entertainment
- Media
- Digital Collectibles
- Animation
- Consumer
- Webhook
---
