---
api_key_in: []
api_specs:
- filename: nabis-platform-api-v2-openapi.yml
  format: yaml
  label: Nabis Platform API v2
  slug: nabis-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-platform-api-v2-openapi.yml
- filename: nabis-platform-api-v1-openapi.json
  format: json
  label: Nabis Platform API v1 (deprecated)
  slug: nabis-platform-api-v1-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-platform-api-v1-openapi.json
- filename: nabis-universal-qr-code-openapi.yaml
  format: yaml
  label: Nabis Universal QR Code API (design specification)
  slug: nabis-universal-qr-code-api-design-specification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-universal-qr-code-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Nabis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nabis declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nabis
provider_slug: nabis
scheme_count: 1
schemes:
- applies_to:
  - Nabis Platform API v2 (https://platform-api.nabis.pro)
  - Nabis Platform API v1 (https://api.getnabis.com/platform/v1) — deprecated
  declared_in_spec: true
  docs: https://developers.nabis.com/v2/docs/overview/authentication
  id: x-nabis-access-token
  in: header
  name: x-nabis-access-token
  notes: Non-standard header name (not RFC 6750 Bearer, not RFC 7617 Basic). The token is a single opaque string with no prefix that distinguishes test from live; there is no test mode.
  spec_location: openapi/nabis-platform-api-v2-openapi.yml#/components/securitySchemes
  type: apiKey
slug: nabis-authentication
source_filename: nabis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developers.nabis.com/v2/docs/overview/authentication\nname: Nabis Platform API — Authentication Profile\ndocs: https://developers.nabis.com/v2/docs/overview/authentication\nsummary: >-\n  The Nabis Platform API (v1 and v2) is secured by a single static API token passed in a custom\n  request header. There is no OAuth 2.0, no OpenID Connect, no mutual TLS and no scope surface.\n  Keys are self-service for California organizations from inside the Nabis application; New York\n  keys are issued by a human via partnerships@nabis.com.\nschemes:\n  - id: x-nabis-access-token\n    type: apiKey\n    in: header\n    name: x-nabis-access-token\n    applies_to:\n      - Nabis Platform API v2 (https://platform-api.nabis.pro)\n      - Nabis Platform API v1 (https://api.getnabis.com/platform/v1) — deprecated\n    declared_in_spec: true\n    spec_location: openapi/nabis-platform-api-v2-openapi.yml#/components/securitySchemes\n    docs:\
  \ https://developers.nabis.com/v2/docs/overview/authentication\n    notes: >-\n      Non-standard header name (not RFC 6750 Bearer, not RFC 7617 Basic). The token is a single\n      opaque string with no prefix that distinguishes test from live; there is no test mode.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  supported: false\n  note: >-\n    The API publishes no scopes, roles or permissions surface. Access is all-or-nothing per key and\n    is implicitly bounded by the organization the key belongs to. scopes/ is therefore not emitted.\nkey_management:\n  self_service: partial\n  provisioning_docs: https://developers.nabis.com/v2/docs/overview/generating-api-key\n  steps:\n    - Log in to the Nabis app (https://app.nabis.com)\n    - Left-hand navigation → Team\n    - Tabs across the page → API\n    - Generate API Key, name it, Save\n  california: self-service in the Nabis application\n  new_york: request via partnerships@nabis.com (not self-service)\n  general_access_request:\
  \ help@nabis.com\n  rotation_policy_published: false\n  expiry_published: false\n  multiple_keys: true\n  key_naming: Keys are named by the operator and listed per organization in the app\naudit:\n  available: true\n  docs: https://developers.nabis.com/v2/docs/overview/audit-logs\n  detail: >-\n    Nabis records every API request and exposes a per-key request log (path, status code) in the\n    application UI under Team → API → Logs. Documented as available only in the legacy California\n    application.\nfailure_modes:\n  - status: 401\n    body: '{\"statusCode\": 401, \"message\": \"Invalid API key\"}'\n    cause: Token missing, malformed or revoked\n    source: https://developers.nabis.com/v2/docs/overview/authentication\n  - status: 401\n    body: '{\"statusCode\": 401, \"message\": \"Unauthorized\"}'\n    cause: Observed live on an unauthenticated GET https://platform-api.nabis.pro/v2/nabis-days-off\n    source: probed 2026-08-26\ntransport_security:\n  https_only: true\n  hsts: true\n\
  \  observed_headers:\n    - Strict-Transport-Security: max-age=15552000; includeSubDomains\n    - Content-Security-Policy (default-src 'self')\n    - X-Content-Type-Options: nosniff\n    - Referrer-Policy: no-referrer\n    - X-Frame-Options: SAMEORIGIN\n    - Cross-Origin-Opener-Policy: same-origin\n  observed_on: https://platform-api.nabis.pro/v2/nabis-days-off\n  observed_date: '2026-08-26'\ngaps:\n  - No published key rotation or expiry policy.\n  - No OAuth 2.0 or delegated-authorization path, so no third-party app can act on a retailer's or\n    brand's behalf without that organization handing over a long-lived static token.\n  - New York key issuance is not self-service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/authentication/nabis-authentication.yml
summary_line: 1 scheme
tags:
- Cannabis
- Distribution
- Wholesale
- Marketplace
- Logistics
- Supply Chain
- Inventory
- Orders
- Invoicing
- Retail
- Compliance
- Track and Trace
- California
- New York
---
