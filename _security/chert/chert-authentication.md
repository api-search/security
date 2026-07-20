---
api_key_in:
- header
auth_types:
- http
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Chert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chert secures its APIs with http and hmac across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chert
provider_slug: chert
scheme_count: 2
schemes:
- format: Bearer <signing_secret>
  header: authorization
  name: BearerToken
  notes: Simplest method for scripts, prototypes, and trusted server-to-server calls. Signing secret is a 32-char hex value revealed once in the Chert console; server uses constant-time comparison.
  scheme: bearer
  type: http
- algorithm: HMAC-SHA256
  header: x-chert-signature
  header_format: v1,<unix_seconds>,<hmac_hex>
  name: HMAC-SHA256
  raw_body_rules:
  - POST uses the exact transmitted bytes (no re-serialization)
  - GET uses an empty string (signature ends with a trailing dot)
  recommended_for: exposed environments (edge functions, client-side code)
  replay_window_seconds: 300
  signing_string: <unix_seconds>.<raw_body>
  type: hmac
slug: chert-authentication
source_filename: chert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.trychert.com/api/authentication\ndocs: https://docs.trychert.com/api/authentication\nsummary:\n  types: [http, hmac]\n  api_key_in: [header]\n  transport_requirement: TLS 1.2+\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  header: authorization\n  format: \"Bearer <signing_secret>\"\n  notes: >-\n    Simplest method for scripts, prototypes, and trusted server-to-server calls.\n    Signing secret is a 32-char hex value revealed once in the Chert console; server\n    uses constant-time comparison.\n- name: HMAC-SHA256\n  type: hmac\n  algorithm: HMAC-SHA256\n  header: x-chert-signature\n  header_format: \"v1,<unix_seconds>,<hmac_hex>\"\n  signing_string: \"<unix_seconds>.<raw_body>\"\n  raw_body_rules:\n  - POST uses the exact transmitted bytes (no re-serialization)\n  - GET uses an empty string (signature ends with a trailing dot)\n  replay_window_seconds: 300\n  recommended_for: exposed environments\
  \ (edge functions, client-side code)\nrequired_headers:\n- name: x-chert-tenant\n  value: tenant_slug from registration\n  required_when: with HMAC signatures or for multi-tenant accounts\n- name: content-type\n  value: application/json\n  required_when: POST requests\nkey_management:\n  issuance: Signing secret displayed once at registration via the Chert console\n  rotation: Requires contacting a Chert administrator (API keys page -> Reveal/rotate)\n  re_registration: Re-registering the same email returns the existing tenant without regeneration\nwebhook_signing:\n  scheme: HMAC-SHA256\n  note: >-\n    Webhook deliveries use a separate per-subscription secret, computed identically as\n    HMAC-SHA256(subscription_secret, \"<ts>.<raw_body>\"). Do not use the API signing secret\n    to verify webhooks.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chert/refs/heads/main/authentication/chert-authentication.yml
summary_line: http/hmac · 2 schemes
tags:
- Company
- Messaging
- iMessage
- Communications
- Conversational
- Webhooks
- CRM Integration
- API
---
