---
api_key_in:
- header
auth_types:
- apiKey
- httpMessageSignatures
description: ''
kind: authentication
layout: security
method: searched
name: Finmid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finmid secures its APIs with apiKey and httpMessageSignatures across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finmid
provider_slug: finmid
scheme_count: 2
schemes:
- applies_to:
  - B2B Payments API
  - Capital API
  description: Primary authentication for both the B2B Payments API and the Capital API. Every request must include the X-API-Key header. Keys are environment specific — a sandbox key (https://sandbox.finmid.com) cannot access live data and a live key (https://api.finmid.com) cannot access sandbox data. Keys are managed in the finmid Dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  type: apiKey
- algorithm: Ed25519
  applies_to:
  - Capital API - platform-provided capital
  description: For platform-provided capital, the Execute Payment Transaction endpoint (platform-initiated payouts) is additionally protected with HTTP Message Signatures (RFC 9421). Requests are signed with Ed25519, include a Content-Digest for body integrity, use temporal/replay-attack prevention, and require IP whitelisting.
  name: HttpMessageSignatures
  standard: RFC 9421
  type: http-message-signatures
slug: finmid-authentication
source_filename: finmid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.finmid.com/reference/api-introduction\ndocs: https://docs.finmid.com/reference/api-introduction\nsummary:\n  types: [apiKey, httpMessageSignatures]\n  api_key_in: [header]\n  api_key_name: X-API-Key\n  environments: [sandbox, live]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Primary authentication for both the B2B Payments API and the Capital API.\n    Every request must include the X-API-Key header. Keys are environment\n    specific — a sandbox key (https://sandbox.finmid.com) cannot access live\n    data and a live key (https://api.finmid.com) cannot access sandbox data.\n    Keys are managed in the finmid Dashboard.\n  applies_to: [B2B Payments API, Capital API]\n- name: HttpMessageSignatures\n  type: http-message-signatures\n  standard: RFC 9421\n  algorithm: Ed25519\n  description: >-\n    For platform-provided capital, the Execute Payment Transaction\
  \ endpoint\n    (platform-initiated payouts) is additionally protected with HTTP Message\n    Signatures (RFC 9421). Requests are signed with Ed25519, include a\n    Content-Digest for body integrity, use temporal/replay-attack prevention,\n    and require IP whitelisting.\n  applies_to: [Capital API - platform-provided capital]\nwebhook_auth:\n  description: >-\n    Inbound webhooks from finmid to your endpoint use HTTP Basic authentication\n    plus an HMAC-SHA-256 payload signature carried in the X-Payload-Signature\n    header (Base64-encoded), verified with a per-endpoint signature_secret.\n  source: https://docs.finmid.com/docs/webhooks\nnotes:\n- OAuth 2.0 / OpenID Connect are not used — authentication is API-key based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/authentication/finmid-authentication.yml
summary_line: apiKey/httpMessageSignatures · 2 schemes
tags:
- Company
- Embedded Finance
- Embedded Lending
- B2B Payments
- Fintech
- Lending
- Capital
- Financing
- Payments
- Marketplaces
---
