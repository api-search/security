---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actionstreamer-openapi-original.json
  format: json
  label: ActionStreamer Web API
  slug: actionstreamer-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionstreamer/refs/heads/main/openapi/_original/actionstreamer-openapi-original.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Actionstreamer Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActionStreamer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ActionStreamer
provider_slug: actionstreamer
scheme_count: 2
schemes:
- algorithm: HMAC-SHA256, hex digest
  canonical_string:
    joined_with: newline
    order:
    - METHOD
    - PATH
    - HEADER_STRING
    - PARAMETER_STRING
    - BODY
    rules:
    - Content-Type is removed from the header set before signing.
    - Header keys are sorted and rendered as 'key: value' lines.
    - Query or form parameters are sorted and rendered the same way.
    - The path is normalized to start with '/' with no trailing slash, except for root.
    - The assembled string is trimmed before signing.
  credentials:
    access_key: created in the ActionStreamer portal under Settings > API Keys
    provisioning_api: POST /v1/apikey (the API can mint its own keys once authenticated)
    provisioning_url: https://portal.actionstreamer.com
    secret_key: issued alongside the access key; never transmitted
  description: HMAC-SHA256 key/secret request signing, used for headless devices and direct service integrations. The caller derives a hex digest over a canonical string built from the method, path, sorted headers, sorted parameters and body, keyed with the account secret.
  headers_required:
  - name: Authorization
    value: HMAC-SHA256 {access_key}
  - name: X-AccessKey
    value: the access key
  - name: X-Signature
    value: hex-encoded HMAC-SHA256 digest of the canonical string
  - name: X-Timestamp
    value: Unix epoch seconds
  - name: X-Nonce
    value: a UUIDv4, unique per request
  - name: Content-Type
    value: application/json
  http_scheme: HMAC-SHA256
  id: hmac-sha256
  in: header
  reference_implementation: The guide publishes a Python get_hmac_signature(secret_key, method, path, headers, parameters, body) reference function; the first-party PyPI package `actionstreamer` implements it.
  replay_protection:
    mechanism: X-Nonce (UUIDv4 per request) plus X-Timestamp
    note: This is anti-replay for the auth envelope. It is NOT request idempotency — a client that retries a write with a fresh nonce will execute the write twice. See conventions/actionstreamer-conventions.yml.
  type: signature
- description: Session-token authentication used by the ActionStreamer web portal and browser clients, as an alternative to HMAC signing for interactive sessions.
  expiry_signal: HTTP 419 Session expired
  id: session-token
  in: header
  mfa: A MultifactorAuth resource area with nine operations is published, so the platform supports MFA on interactive sessions.
  related_operations:
  - POST /v1/session
  - GET /v1/session
  - POST /v1/token/mediarouter/publish
  - POST /v1/multifactorauth
  type: token
slug: actionstreamer-authentication
source_filename: actionstreamer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.actionstreamer.com/docs/Guides/authentication\ndocs: https://developer.actionstreamer.com/docs/Guides/authentication\nnote: >-\n  Authored from the provider's own authentication guide, NOT derived from the OpenAPI. The published\n  specification declares no components.securitySchemes at all — the developer portal's own overview\n  page states \"securitySchemes declared: False\" — so derive-authentication.py produced nothing for\n  this provider. Everything below is read from the human-readable guide. This is the single largest\n  contract-quality gap in the ActionStreamer surface: the API is authenticated, the auth is\n  documented in prose, and a machine reading only the spec cannot tell.\nscheme_count: 2\nprimary_scheme: hmac-signature\nschemes:\n- id: hmac-sha256\n  type: signature\n  http_scheme: HMAC-SHA256\n  in: header\n  description: >-\n    HMAC-SHA256 key/secret request signing, used for headless\
  \ devices and direct service\n    integrations. The caller derives a hex digest over a canonical string built from the method,\n    path, sorted headers, sorted parameters and body, keyed with the account secret.\n  credentials:\n    access_key: created in the ActionStreamer portal under Settings > API Keys\n    secret_key: issued alongside the access key; never transmitted\n    provisioning_url: https://portal.actionstreamer.com\n    provisioning_api: POST /v1/apikey (the API can mint its own keys once authenticated)\n  headers_required:\n  - name: Authorization\n    value: 'HMAC-SHA256 {access_key}'\n  - name: X-AccessKey\n    value: the access key\n  - name: X-Signature\n    value: hex-encoded HMAC-SHA256 digest of the canonical string\n  - name: X-Timestamp\n    value: Unix epoch seconds\n  - name: X-Nonce\n    value: a UUIDv4, unique per request\n  - name: Content-Type\n    value: application/json\n  canonical_string:\n    order:\n    - METHOD\n    - PATH\n    - HEADER_STRING\n  \
  \  - PARAMETER_STRING\n    - BODY\n    joined_with: newline\n    rules:\n    - Content-Type is removed from the header set before signing.\n    - Header keys are sorted and rendered as 'key: value' lines.\n    - Query or form parameters are sorted and rendered the same way.\n    - The path is normalized to start with '/' with no trailing slash, except for root.\n    - The assembled string is trimmed before signing.\n  algorithm: HMAC-SHA256, hex digest\n  replay_protection:\n    mechanism: X-Nonce (UUIDv4 per request) plus X-Timestamp\n    note: >-\n      This is anti-replay for the auth envelope. It is NOT request idempotency — a client that\n      retries a write with a fresh nonce will execute the write twice. See\n      conventions/actionstreamer-conventions.yml.\n  reference_implementation: >-\n    The guide publishes a Python get_hmac_signature(secret_key, method, path, headers, parameters,\n    body) reference function; the first-party PyPI package `actionstreamer` implements it.\n\
  - id: session-token\n  type: token\n  in: header\n  description: >-\n    Session-token authentication used by the ActionStreamer web portal and browser clients, as an\n    alternative to HMAC signing for interactive sessions.\n  related_operations:\n  - POST /v1/session\n  - GET /v1/session\n  - POST /v1/token/mediarouter/publish\n  - POST /v1/multifactorauth\n  expiry_signal: HTTP 419 Session expired\n  mfa: >-\n    A MultifactorAuth resource area with nine operations is published, so the platform supports MFA\n    on interactive sessions.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_header: false\nspec_gap:\n  securitySchemes_declared: false\n  security_applied_to_operations: false\n  operations_total: 247\n  operations_with_security: 0\n  impact: >-\n    Every generated client, agent tool wrapper and API-explorer built from this OpenAPI will emit\n    unauthenticated requests. Declaring an apiKey-in-header scheme for X-AccessKey/X-Signature (or a\n    documented\
  \ custom scheme) and applying it at the root `security` level would close this without\n    changing a single operation.\nrecommendations:\n- Declare components.securitySchemes in the published OpenAPI and apply a root-level security requirement.\n- Publish the key rotation and revocation policy; DELETE /v1/apikey/{apiKeyID} exists but no lifecycle guidance accompanies it.\n- Document the accepted clock skew for X-Timestamp so clients know how far out of sync they may drift.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionstreamer/refs/heads/main/authentication/actionstreamer-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Live Streaming
- Wearables
- Internet of Things
- Device Management
- Public Safety
- Industrial
- Computer Vision
- Media
---
