---
api_key_in:
- header
api_specs:
- filename: tempmailgrab-openapi.json
  format: json
  label: TempMailGrab REST API
  slug: tempmailgrab-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tempmailgrab/refs/heads/main/openapi/tempmailgrab-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tempmailgrab Authentication
name_suffix: Authentication
oauth_flows: []
overview: TempMailGrab API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TempMailGrab API
provider_slug: tempmailgrab
scheme_count: 2
schemes:
- header: 'Authorization: Bearer tmg_live_xxx'
  key_prefix: tmg_live_
  name: bearerAuth
  preferred: true
  scheme: bearer
  sources:
  - openapi/tempmailgrab-openapi.json
  - https://tempmailgrab.com/api-docs
  type: http
- header: 'X-API-Key: tmg_live_xxx'
  in: header
  key_prefix: tmg_live_
  legacy: true
  name: apiKey
  note: /api-docs calls this "the legacy header" and states both work on every request.
  parameter: X-API-Key
  sources:
  - openapi/tempmailgrab-openapi.json
  - https://tempmailgrab.com/api-docs
  type: apiKey
slug: tempmailgrab-authentication
source_filename: tempmailgrab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://tempmailgrab.com/api-docs\nderived_from: openapi/tempmailgrab-openapi.json\nalso: https://tempmailgrab.com/security\ndocs: https://tempmailgrab.com/api-docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  applied: >-\n    Both schemes are applied at the document level as alternatives - security is\n    [{bearerAuth: []}, {apiKey: []}] - so every one of the 15 operations requires a key and either header\n    form is accepted.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer tmg_live_xxx'\n  key_prefix: tmg_live_\n  preferred: true\n  sources:\n  - openapi/tempmailgrab-openapi.json\n  - https://tempmailgrab.com/api-docs\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  header: 'X-API-Key: tmg_live_xxx'\n  key_prefix: tmg_live_\n  legacy: true\n  note: '/api-docs calls\
  \ this \"the legacy header\" and states both work on every request.'\n  sources:\n  - openapi/tempmailgrab-openapi.json\n  - https://tempmailgrab.com/api-docs\nkey_management:\n  issuance: >-\n    Create a free account on the developer dashboard (email/password or GitHub sign-in), then mint an API\n    key. Every key is tied to the account, so keys and the dashboard share the same private inboxes.\n  dashboard: https://tempmailgrab.com/dashboard\n  sign_in_methods:\n  - email/password\n  - GitHub\n  rotation: >-\n    Keys can be rotated from the dashboard. The provider advises rotating immediately on suspected exposure\n    rather than waiting to confirm misuse.\n  scoping: >-\n    Account-scoped bearer credential - anyone holding it can act as the account. There are no scopes,\n    no per-key permissions, and no read-only key class.\n  storage_guidance: >-\n    \"Keep it in an environment variable or your CI provider's secret store, never in committed source, and\n    never in client-side\
  \ code where a browser would expose it.\" (https://tempmailgrab.com/security)\n  transport: TLS only.\nauthorization:\n  model: ownership\n  description: >-\n    Inboxes are private to the key's account; another key cannot read your mail. There is no scope, role, or\n    consent surface - authorization is entirely \"did this key create this resource\".\n  scopes_published: false\nrate_limit_binding: >-\n  Limits are enforced per API key rather than per IP, so a CI runner behind shared NAT gets its own budget.\n  See rate-limits/tempmailgrab-rate-limits.yml.\nwebhook_authentication:\n  outbound: HMAC-SHA256 over the raw body in X-TMG-Signature, keyed by a whsec_ secret returned once at\n    webhook creation.\n  see: asyncapi/tempmailgrab-webhooks.yml\nnegative_probes:\n- url: https://tempmailgrab.com/.well-known/openid-configuration\n  status: 404\n- url: https://tempmailgrab.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://tempmailgrab.com/.well-known/oauth-protected-resource\n\
  \  status: 404\n- url: https://tempmailgrab.com/api/v1/openapi.json\n  status: 401\n  note: Confirms every /api/v1 path is gated - an unauthenticated call returns 401, not a public error page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempmailgrab/refs/heads/main/authentication/tempmailgrab-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- email
- temporary-email
- disposable-email
- otp
- webhooks
- qa
- testing
- playwright
- cypress
- developer-tools
- email-testing
- ci
---
