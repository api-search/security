---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Dunamu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dunamu declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dunamu
provider_slug: dunamu
scheme_count: 1
schemes:
- algorithm: HS256
  bearerFormat: JWT
  claims:
  - description: The issued access key.
    name: access_key
    required: true
  - description: A random UUID string, unique per request. Reuse is rejected with error code `nonce_used`.
    name: nonce
    required: true
  - description: Hash of the request query string. Required only when the request carries parameters. The query string must be a standard URL query string — JSON is not permitted for hashing.
    name: query_hash
    required: conditional
  - description: Algorithm used for query_hash. SHA512.
    name: query_hash_alg
    required: conditional
  deprecated_predecessor: The legacy `query` claim form was deprecated in March 2022 in favour of query_hash + query_hash_alg.
  header: Authorization
  header_form: 'Authorization: Bearer <jwt>'
  id: upbit-jwt
  scheme: bearer
  signing_key: The issued secret key, used raw. The documentation states explicitly that "the issued secret key is not base64 encoded" and warns developers to check their JWT library settings.
  type: http
slug: dunamu-authentication
source_filename: dunamu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://global-docs.upbit.com/reference/auth\ndocs: https://global-docs.upbit.com/docs/api-key\nnote: >-\n  Authentication profile for the developer surface Dunamu Inc. operates under the Upbit brand.\n  Dunamu itself serves no authenticated API from dunamu.com. Read from the Upbit Developer Center\n  reference and its markdown twins (/reference/auth.md, /reference/rest-api-guide.md,\n  /docs/api-key.md) on 2026-08-12. No OpenAPI securityScheme block was available to derive from —\n  the Dunamu record carries no OpenAPI (the spec set lives on the Upbit provider profile), so this\n  is a docs-sourced profile, not a spec derivation.\nx-brand: Upbit\nsurfaces:\n- name: Quotation API\n  scope: public market data\n  authentication: none\n  note: >-\n    Public API, accessible without authentication. Read-only (trading pairs, candles, trade\n    history, tickers, orderbooks).\n- name: Exchange API\n  scope: accounts, orders, deposits,\
  \ withdrawals, travel rule\n  authentication: jwt-bearer\n  note: Private API. API Key required. Create, Read, Delete (cancel) operations.\nschemes:\n- id: upbit-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: Authorization\n  header_form: 'Authorization: Bearer <jwt>'\n  algorithm: HS256\n  signing_key: >-\n    The issued secret key, used raw. The documentation states explicitly that \"the issued secret\n    key is not base64 encoded\" and warns developers to check their JWT library settings.\n  claims:\n  - name: access_key\n    required: true\n    description: The issued access key.\n  - name: nonce\n    required: true\n    description: >-\n      A random UUID string, unique per request. Reuse is rejected with error code `nonce_used`.\n  - name: query_hash\n    required: conditional\n    description: >-\n      Hash of the request query string. Required only when the request carries parameters. The\n      query string must be a standard URL query string — JSON is\
  \ not permitted for hashing.\n  - name: query_hash_alg\n    required: conditional\n    description: Algorithm used for query_hash. SHA512.\n  deprecated_predecessor: >-\n    The legacy `query` claim form was deprecated in March 2022 in favour of\n    query_hash + query_hash_alg.\nkey_management:\n  issuance_url: https://global-docs.upbit.com/docs/api-key\n  issuance_path: 'Upbit PC web > My Profile > Open API'\n  issuance_constraint: >-\n    \"API Keys can be issued only through the PC web interface and require a security level of 2 or\n    higher.\" Not issuable from mobile.\n  permissions:\n  - id: view-assets\n    description: Read account assets and balances.\n    ip_allowlist_required: false\n  - id: make-orders\n    description: Create and cancel orders.\n    ip_allowlist_required: true\n  - id: withdraw\n    description: Request digital asset withdrawals.\n    ip_allowlist_required: true\n  ip_allowlist:\n    required_for: [make-orders, withdraw]\n    rule: >-\n      \"If you select\
  \ Make Orders or Withdraw, you must register an allowlisted IP address.\"\n      A static IP is mandatory — the FAQ states dynamic-IP environments are not supported for\n      key-authenticated Exchange APIs because they involve deposits, withdrawals and trading.\n    error_on_mismatch: no_authorization_ip (HTTP 401)\n  expiry:\n    documented_period: null\n    note: >-\n      The docs expose an \"Expired Keys\" tab for deleting expired keys and an `expired_access_key`\n      (HTTP 401) error code, so keys DO expire — but no validity period is stated on the API-key\n      page. Recorded as an honest gap, not guessed.\noauth2:\n  supported: false\n  note: >-\n    No OAuth 2.0, no OpenID Connect, no authorization-server metadata. Probed 2026-08-12:\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration return 404 on\n    global-docs.upbit.com and dunamu.com. No scopes/ artifact is emitted for this provider —\n    permissions are key-level checkboxes set at issuance,\
  \ not OAuth scopes. The single\n    scope-shaped runtime signal is the `out_of_scope` error code (HTTP 403), which reports that a\n    key lacks the permission for the requested operation.\ntransport:\n  tls_minimum: TLSv1.2\n  tls_recommended: TLSv1.3\n  note: >-\n    \"The Upbit Open API supports only TLS version 1.2 or higher.\" Versions below TLS 1.2 are\n    stated as no longer supported.\nwebsocket:\n  authentication: >-\n    Private WebSocket streams (wss://<region>-api.upbit.com/websocket/v1/private) use the same JWT\n    bearer token as the REST Exchange API. Public streams\n    (wss://<region>-api.upbit.com/websocket/v1) require no authentication.\n  docs: https://global-docs.upbit.com/reference/websocket-guide\nerrors:\n  reference: errors/dunamu-problem-types.yml\n  auth_codes:\n  - invalid_query_payload\n  - jwt_verification\n  - expired_access_key\n  - nonce_used\n  - no_authorization_ip\n  - no_authorization_token\n  - out_of_scope\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dunamu/refs/heads/main/authentication/dunamu-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Cryptocurrency
- Digital Assets
- Exchange
- Securities
- Trading
- Blockchain
- South Korea
- Company
---
