---
api_key_in:
- header
api_specs:
- filename: convelio-shipping-api-openapi.yml
  format: yaml
  label: Convelio Shipping API
  slug: convelio-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/openapi/convelio-shipping-api-openapi.yml
- filename: convelio-webhook-api-openapi.yml
  format: yaml
  label: Convelio Webhook API
  slug: convelio-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/openapi/convelio-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Convelio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convelio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convelio
provider_slug: convelio
scheme_count: 2
schemes:
- applied_to: all documented operations (declared as the document-level default security)
  description: Account secret API key. Prefixed `sk`. Convelio documents it as a Secret-type key that "should be kept confidential and only stored on your own servers" and that "can perform any API request to Convelio without restriction" — there is no restricted/publishable key tier and no per-scope narrowing.
  format: token <secret_key>
  in: header
  name: secret_token
  parameter: Authorization
  sources:
  - openapi/convelio-shipping-openapi.yml
  type: apiKey
- description: HMAC-SHA256 signature computed over the webhook body with the account's API secret token. Present on webhook callbacks Convelio POSTs to a subscriber URL, for verification by the receiver — not sent by clients on API requests.
  direction: inbound-to-subscriber
  in: header
  name: convelio_signature
  parameter: X-Convelio-signature
  sources:
  - openapi/convelio-shipping-openapi.yml
  type: apiKey
slug: convelio-authentication
source_filename: convelio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/convelio-shipping-openapi.yml\ndocs: https://developers.convelio.com/#section/API-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Convelio authenticates every Shipping API request with a single secret API key\n    presented in the Authorization header using the literal form `token <secret>`.\n    There is no OAuth 2.0, no OpenID Connect, and no scope surface — the key is\n    all-or-nothing. A second apiKey scheme, X-Convelio-signature, is not a request\n    credential at all: it is the HMAC-SHA256 signature Convelio attaches to OUTBOUND\n    webhook deliveries so the receiver can verify them.\nschemes:\n- name: secret_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: token <secret_key>\n  description: >-\n    Account secret API key. Prefixed `sk`. Convelio documents it as a Secret-type key\n    that \"should be kept confidential and only\
  \ stored on your own servers\" and that\n    \"can perform any API request to Convelio without restriction\" — there is no\n    restricted/publishable key tier and no per-scope narrowing.\n  applied_to: all documented operations (declared as the document-level default security)\n  sources:\n  - openapi/convelio-shipping-openapi.yml\n- name: convelio_signature\n  type: apiKey\n  in: header\n  parameter: X-Convelio-signature\n  direction: inbound-to-subscriber\n  description: >-\n    HMAC-SHA256 signature computed over the webhook body with the account's API secret\n    token. Present on webhook callbacks Convelio POSTs to a subscriber URL, for\n    verification by the receiver — not sent by clients on API requests.\n  sources:\n  - openapi/convelio-shipping-openapi.yml\nkey_modes:\n  scheme: prefix-encoded mode selection\n  description: >-\n    The key itself, not a separate parameter, selects the environment. A test key only\n    works against the sandbox server; a live key only works\
  \ against production.\n  keys:\n  - mode: test\n    prefix: sk_test_\n    server: https://api.sandbox.convelio.com/v2\n  - mode: live\n    prefix: sk_live_\n    server: https://api.convelio.com/v2\nprovisioning:\n  self_service: false\n  method: email request\n  contact: api@convelio.com\n  note: >-\n    Keys are not self-service. Convelio's documentation states \"To get your API key,\n    please send your request at api@convelio.com.\" There is no developer console that\n    mints a key, so the credential path is gated on a human at Convelio.\ngaps:\n- No OAuth 2.0 / OpenID Connect surface; no delegated or third-party authorization.\n- No scoped or restricted keys — a single secret key grants the full API surface.\n- No documented key rotation, expiry, or revocation procedure.\n- No self-service key issuance; provisioning is an email round-trip.\n- No mTLS, no proof-of-possession, no request signing on inbound requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/authentication/convelio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Logistics
- Shipping
- Fine Art
- Freight
- Ecommerce
- Quotes
- Webhooks
- Customs
- Insurance
---
