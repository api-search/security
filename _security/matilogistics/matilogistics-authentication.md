---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Matilogistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mati Logistics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mati Logistics
provider_slug: matilogistics
scheme_count: 1
schemes:
- description: Every request requires a bearer token in the Authorization header. Keys are issued per organization and scoped to it, so a key can only ever read and write that organization's own shipments.
  example_shape: tnt_your_key_here
  format: 'Authorization: Bearer <key>'
  header: Authorization
  id: bearer
  in: header
  key_prefix: tnt_
  required: true
  scheme: bearer
  type: http
slug: matilogistics-authentication
source_filename: matilogistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://www.matilogistics.com/api — the \"Authentication\" and \"Getting access\"\n  sections of the published API Reference, read on 2026-08-27. Mati Logistics\n  publishes NO OpenAPI, so this profile could not be derived from\n  securitySchemes; every field below is quoted from the provider's own prose\n  reference, and the 401 envelope was confirmed against a live unauthenticated\n  request to https://api.matilogistics.com/v2/carriers.\ndocs: https://www.matilogistics.com/api#access\nprovider: Mati Logistics\nproviderId: matilogistics\napi: Mati Logistics Track and Trace API\nbase_url: https://api.matilogistics.com\n\nschemes:\n  - id: bearer\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <key>'\n    key_prefix: tnt_\n    example_shape: tnt_your_key_here\n    description: >-\n      Every request requires a bearer token in the Authorization header.\
  \ Keys\n      are issued per organization and scoped to it, so a key can only ever read\n      and write that organization's own shipments.\n    required: true\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nbasic_auth: false\napi_key_query_param: false\n\nkey_management:\n  issued_from: The API keys page inside the Mati web app (app.matilogistics.com / /app)\n  availability: Any subscription plan; a 7-day free trial is available.\n  scope: Per organization.\n  display: >-\n    \"Your key is shown exactly once when issued and is not recoverable\n    afterwards; if you lose it, revoke it and issue a new one.\"\n  rotation: Revoke and issue a new key. No programmatic key-management API is documented.\n  self_service: true\n  gating: >-\n    API access is not on the free / pay-as-you-go tier. It is included with\n    subscriptions of 250+ shipments per month, or purchasable for $1,800 per\n    year on lower-volume subscriptions. See plans/matilogistics-plans-pricing.yml.\n\nimpersonation:\n\
  \  supported: true\n  note: >-\n    The published 403 meaning — \"The key is not permitted to act as the\n    subscriber it named\" — indicates a key may name a subscriber it acts for,\n    but the mechanism (header or body field) is NOT documented in the public\n    reference.\n\nwebhook_authentication:\n  direction: outbound (Mati -> your endpoint)\n  scheme: HMAC-SHA256\n  signature_header: X-TNT-Signature\n  event_header: X-TNT-Event\n  encoding: hex\n  signed_payload: the raw request body, before JSON parsing or re-serialization\n  secret: >-\n    Per-endpoint signing secret returned once at webhook creation; may be\n    supplied at creation or rotated via POST /v2/webhooks/{id}/rotate_secret.\n  docs: https://www.matilogistics.com/api\n\nfailure_responses:\n  - status: 401\n    code: unauthenticated\n    meaning: Missing, invalid, or revoked API key.\n    observed_body: '{\"error\":{\"code\":\"unauthenticated\",\"message\":\"Missing bearer token\",\"request_id\":\"...\"},\"detail\"\
  :\"Missing bearer token\"}'\n    observed_at: 'https://api.matilogistics.com/v2/carriers (probed 2026-08-27, no Authorization header)'\n  - status: 403\n    meaning: The key is not permitted to act as the subscriber it named.\n  - status: 404\n    meaning: No such object, or one outside the requesting organization.\n\nevidence:\n  - url: https://www.matilogistics.com/api\n    status: 200\n    note: Server-rendered HTML reference containing the Authentication section verbatim.\n  - url: https://api.matilogistics.com/v2/carriers\n    status: 401\n    note: Live unauthenticated probe; returned the documented unauthenticated envelope.\n  - url: https://api.matilogistics.com/.well-known/oauth-authorization-server\n    status: 404\n    note: No OAuth authorization-server metadata; bearer API keys are the only scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matilogistics/refs/heads/main/authentication/matilogistics-authentication.yml
summary_line: 1 scheme
tags:
- Logistics
- Supply Chain
- Shipping
- Container Tracking
- Ocean Freight
- Track and Trace
- Shipment Visibility
- Freight Forwarding
- NVOCC
- Webhook
- REST
- Procurement
---
