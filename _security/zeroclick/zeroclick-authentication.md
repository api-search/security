---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Zeroclick Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeroclick declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zeroclick
provider_slug: zeroclick
scheme_count: 2
schemes:
- description: Scoped API key created in the ZeroClick dashboard and supplied to the seller SDK (ZEROCLICK_API_KEY). Used for allowance checks and usage reporting.
  id: api_key
  in: header
  scope_notes: Use admin:* keys for tooling that manages configuration; use a separate key with both usage:read and usage:write for the server integration. Legacy billing:* and secrets:* scopes were migrated to the equivalent admin:* scopes with the same access.
  scopes:
  - grants: Read sellers, services, meters, plans, prices, custom domains, signing-secret metadata, and analytics.
    name: admin:read
  - grants: Create, update, and delete configuration, including creating and revoking signing secrets. Does not imply admin:read.
    name: admin:write
  - grants: Check whether requested usage is allowed.
    name: usage:read
  - grants: Report billable usage.
    name: usage:write
  type: apiKey
- description: ZeroClick signs every proxied request to the seller's upstream so only ZeroClick-signed traffic can reach billable endpoints. Sellers verify the signature over the exact request bytes before doing billable work.
  headers:
  - format: t=<unix-ts>,kid=zcsec_...,v1=<hex-hmac>
    name: zc-signature
  - format: zcreq_...
    name: zc-request-id
  - format: agt_...  (omitted on an anonymous identity probe)
    name: zc-agent-id
  id: request_signature
  in: header
  scheme: hmac
  signing_secret: Per-seller signing secret (zcsec_...) created in the dashboard, shown once. Supports key rotation via kid so in-flight requests signed with either the current or previous secret continue to verify.
  tolerance: Default five-minute signature timestamp tolerance.
  type: http
slug: zeroclick-authentication
source_filename: zeroclick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://zeroclick.ai/docs (Seller Integration Guide)\nsummary: >-\n  ZeroClick sellers authenticate to the ZeroClick API with a scoped API key, and\n  verify inbound proxied agent traffic with an HMAC request signature. There is\n  no OAuth2 flow documented for the seller integration.\nschemes:\n- id: api_key\n  type: apiKey\n  in: header\n  description: >-\n    Scoped API key created in the ZeroClick dashboard and supplied to the seller\n    SDK (ZEROCLICK_API_KEY). Used for allowance checks and usage reporting.\n  scopes:\n  - name: admin:read\n    grants: Read sellers, services, meters, plans, prices, custom domains, signing-secret metadata, and analytics.\n  - name: admin:write\n    grants: Create, update, and delete configuration, including creating and revoking signing secrets. Does not imply admin:read.\n  - name: usage:read\n    grants: Check whether requested usage is allowed.\n  - name: usage:write\n    grants: Report\
  \ billable usage.\n  scope_notes: >-\n    Use admin:* keys for tooling that manages configuration; use a separate key\n    with both usage:read and usage:write for the server integration. Legacy\n    billing:* and secrets:* scopes were migrated to the equivalent admin:*\n    scopes with the same access.\n- id: request_signature\n  type: http\n  scheme: hmac\n  in: header\n  description: >-\n    ZeroClick signs every proxied request to the seller's upstream so only\n    ZeroClick-signed traffic can reach billable endpoints. Sellers verify the\n    signature over the exact request bytes before doing billable work.\n  headers:\n  - name: zc-signature\n    format: t=<unix-ts>,kid=zcsec_...,v1=<hex-hmac>\n  - name: zc-request-id\n    format: zcreq_...\n  - name: zc-agent-id\n    format: agt_...  (omitted on an anonymous identity probe)\n  signing_secret: >-\n    Per-seller signing secret (zcsec_...) created in the dashboard, shown once.\n    Supports key rotation via kid so in-flight requests\
  \ signed with either the\n    current or previous secret continue to verify.\n  tolerance: Default five-minute signature timestamp tolerance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroclick/refs/heads/main/authentication/zeroclick-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Agent Commerce
- Agentic Payments
- API Monetization
- x402
- Machine Payments Protocol
- Agent Identity
- Stripe
---
