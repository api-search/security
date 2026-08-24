---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Gosite Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoSite declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GoSite
provider_slug: gosite
scheme_count: 1
schemes:
- documented: true
  id: api_key
  in: null
  name: null
  note: An API key is issued to an approved requester. The parameter name and location are not published; they would appear only in the gated Swagger reference.
  source: https://developers.gosite.com/api-access
  type: apiKey
slug: gosite-authentication
source_filename: gosite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://developers.gosite.com/api-access\nnote: >-\n  Derived from GoSite's own published access process, NOT from an OpenAPI document — no\n  machine-readable contract could be retrieved (the Swagger host\n  https://api.developers.gosite.com/docs/ returned HTTP 502 on every path on 2026-08-22).\n  GoSite's developer portal states the mechanism explicitly: \"Once your request is\n  approved, we will provide an API Key that will let you make API calls.\" The key's\n  transport (header name, query parameter, or bearer form), its lifetime, rotation and\n  revocation are NOT published anywhere public, so they are recorded as unknown rather\n  than assumed.\nsummary: >-\n  Approval-gated API key. No OAuth, no OpenID Connect, no public self-service credential\n  issuance, and no published scope model.\nschemes:\n- id: api_key\n  type: apiKey\n  name: null\n  in: null\n  documented: true\n  note: >-\n    An API key is issued to an\
  \ approved requester. The parameter name and location are\n    not published; they would appear only in the gated Swagger reference.\n  source: https://developers.gosite.com/api-access\nissuance:\n  model: approval-gated\n  self_service: false\n  steps:\n  - order: 1\n    step: Create a GoSite customer account\n    detail: >-\n      \"You'll need to create a new GoSite customer account to play with and test our\n      APIs\" — an existing commercial relationship with GoSite is a precondition.\n  - order: 2\n    step: Submit the request-access form\n    detail: >-\n      \"Fill out this form to request API access. This will take < 5 mins. Explain why you\n      want access to our APIs.\" The requester must justify the use case.\n  - order: 3\n    step: Receive an API key on approval\n    detail: >-\n      \"Once approved, test out our Swagger APIs. Once your request is approved, we will\n      provide an API Key that will let you make API calls.\"\n  approval_required: true\n  turnaround_published:\
  \ false\noauth:\n  supported: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface is published. The probes of\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server on\n    every GoSite host missed (see well-known/gosite-well-known.yml), so no\n    scopes/ artifact is emitted — there is no scope surface to describe.\nmtls:\n  supported: false\n  documented: false\nobserved:\n- url: https://api.gosite.com/\n  status: 401\n  body: '{\"timestamp\":\"...\",\"status\":401,\"error\":\"Unauthorized\",\"message\":\"\",\"path\":\"/\"}'\n  finding: >-\n    Live authenticated Spring service on GoSite's own domain. It rejects anonymous\n    requests with a JSON 401 envelope and returns NO WWW-Authenticate challenge, so the\n    expected credential form cannot be inferred from the response.\n- url: https://api.developers.gosite.com/docs/\n  status: 502\n  finding: >-\n    The Swagger reference named by GoSite's own developer portal is down; the\n    authentication\
  \ section of the reference could not be read.\ngaps:\n- The API key header/parameter name is not published.\n- No key rotation, expiry or revocation policy is published.\n- No scope or permission model is published.\n- No public reference documents the authentication flow end to end.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gosite/refs/heads/main/authentication/gosite-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Small Business
- Local Services
- Website Builder
- Reputation Management
- Reviews
- Messaging
- Scheduling
- Appointments
- Payments
- Invoicing
- CRM
- Contact Management
- Local SEO
- Home Services
- Field Service
---
