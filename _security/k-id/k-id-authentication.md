---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: K Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: k-ID secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: k-ID
provider_slug: k-id
scheme_count: 1
schemes:
- format: 'Authorization: Bearer {api-key}'
  header: Authorization
  in: header
  issued_via: https://portal.k-id.com
  name: bearerAuth
  scheme: bearer
  scope: per-product
  sources:
  - https://docs.k-id.com/api/authentication
  type: http
slug: k-id-authentication
source_filename: k-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.k-id.com/api/authentication\ndocs: https://docs.k-id.com/api/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Server-to-server only. A per-Product k-ID API key is issued in Compliance\n    Studio (portal.k-id.com) and presented as an HTTP bearer token. Keys must\n    never be exposed in browsers or mobile clients; all calls originate from\n    the integrator's servers over HTTPS.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {api-key}'\n  scope: per-product\n  issued_via: https://portal.k-id.com\n  sources:\n  - https://docs.k-id.com/api/authentication\nwebhook_auth:\n  scheme: hmac-sha256\n  description: >-\n    Inbound webhooks are authenticated by verifying an HMAC-SHA256 signature of\n    the UNIX timestamp concatenated with the raw request body, keyed by the\n\
  \    per-Product webhook secret configured in Compliance Studio.\n  headers:\n  - X-Signature-Timestamp\n  - X-Signature-Hmac-Sha256\n  - X-Event-Type\n  source: https://docs.k-id.com/events/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k-id/refs/heads/main/authentication/k-id-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Age Verification
- Age Assurance
- Compliance
- Parental Consent
- Child Safety
- Identity
- Privacy
- Regulatory Technology
- Gaming
---
