---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Qomplx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qomplx declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Qomplx
provider_slug: qomplx
scheme_count: 2
schemes:
- description: The default scheme. The caller holds an application key (tenant-scoped) or an admin key (key-management scoped) together with a secret key. The Authorization header carries the key identifier plus an HMAC-SHA256 signature.
  header: Authorization
  id: mdtsdb-signature
  in: header
  keys:
  - name: app_key
    scope: tenant data plane — ingest, query, delayed results, websocket
  - name: admin_key
    scope: control plane — /api/v1/admin key lifecycle; also usable on the data plane
  - name: secret_key
    scope: signing material for whichever key is presented; never transmitted
  scheme_prefix: MDTSDB2
  signature:
    algorithm: HMAC-SHA256
    canonical_request: '''/'' + uri + ''\n'' + content_type + ''\n'' + sha256(payload)'
    derivation: A signing key is derived by chained HMAC-SHA256 over the timestamp then the method name, seeded with the secret key.
    replay_window_note: The timestamp is coarse by construction (seconds // 1000, roughly 16.7-minute buckets), which is what the client transmits; the server-side tolerance is not published.
    signed_string: timestamp + '\n' + user_key + '\n' + sha256(canonical_request)
    timestamp: unix seconds integer-divided by 1000 (str(int(time.time()) // 1000))
  type: apiKey-signed
- description: 'An alternative to request signing. The client posts client_id/client_secret with grant_type=client_credentials, application/x-www-form-urlencoded, to a caller-supplied Keycloak token endpoint, then sends `Authorization: Bearer <access_token>` on HTTP and WebSocket requests. The token endpoint URL is deployment-specific and is passed to the client constructor as auth_url.'
  flow: clientCredentials
  id: keycloak-oauth2
  refresh: The client re-requests a token via keycloak_update_access_token() when a response is classified as an authorization error.
  scopes_published: false
  token_endpoint: null
  token_endpoint_note: Deployment-specific (Keycloak realm chosen by the operator); QOMPLX publishes no hosted token endpoint.
  type: oauth2
slug: qomplx-authentication
source_filename: qomplx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: https://github.com/QOMPLX-INC/te-python-client/blob/master/mdtsdb/client.py\nname: QOMPLX TimeEngine authentication\nsummary: >-\n  Derived from QOMPLX's own published TimeEngine Python client. QOMPLX publishes no OpenAPI and\n  no auth documentation page, so every scheme below was read from first-party client source\n  (mdtsdb/client.py) rather than from a docs page. TimeEngine supports two mutually exclusive\n  request-authentication models: a keyed HMAC-SHA256 request signature, and a Keycloak-issued\n  OAuth 2.0 bearer token.\ndocs: null\ndocs_note: >-\n  No public authentication reference exists. www.qomplx.com serves no developer documentation;\n  every content page in its sitemap returns a 301 self-redirect loop.\nschemes:\n- id: mdtsdb-signature\n  type: apiKey-signed\n  in: header\n  header: Authorization\n  scheme_prefix: MDTSDB2\n  description: >-\n    The default scheme. The caller holds an application key (tenant-scoped)\
  \ or an admin key\n    (key-management scoped) together with a secret key. The Authorization header carries the\n    key identifier plus an HMAC-SHA256 signature.\n  signature:\n    algorithm: HMAC-SHA256\n    derivation: >-\n      A signing key is derived by chained HMAC-SHA256 over the timestamp then the method name,\n      seeded with the secret key.\n    canonical_request: \"'/' + uri + '\\\\n' + content_type + '\\\\n' + sha256(payload)\"\n    signed_string: \"timestamp + '\\\\n' + user_key + '\\\\n' + sha256(canonical_request)\"\n    timestamp: \"unix seconds integer-divided by 1000 (str(int(time.time()) // 1000))\"\n    replay_window_note: >-\n      The timestamp is coarse by construction (seconds // 1000, roughly 16.7-minute buckets),\n      which is what the client transmits; the server-side tolerance is not published.\n  keys:\n  - name: app_key\n    scope: tenant data plane — ingest, query, delayed results, websocket\n  - name: admin_key\n    scope: control plane — /api/v1/admin\
  \ key lifecycle; also usable on the data plane\n  - name: secret_key\n    scope: signing material for whichever key is presented; never transmitted\n- id: keycloak-oauth2\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    An alternative to request signing. The client posts client_id/client_secret with\n    grant_type=client_credentials, application/x-www-form-urlencoded, to a caller-supplied\n    Keycloak token endpoint, then sends `Authorization: Bearer <access_token>` on HTTP and\n    WebSocket requests. The token endpoint URL is deployment-specific and is passed to the\n    client constructor as auth_url.\n  token_endpoint: null\n  token_endpoint_note: >-\n    Deployment-specific (Keycloak realm chosen by the operator); QOMPLX publishes no hosted\n    token endpoint.\n  scopes_published: false\n  refresh: >-\n    The client re-requests a token via keycloak_update_access_token() when a response is\n    classified as an authorization error.\nmutual_tls: false\nopenid_connect:\
  \ false\ntransport:\n  https_supported: true\n  https_default: false\n  note: >-\n    The client defaults to plain HTTP (is_https=False, host=127.0.0.1, port=8080). TLS is\n    opt-in and depends on the operator's deployment.\nwebsocket_auth: >-\n  The same two schemes apply to ws(s)://{host}:{port}/api/v1/ws/{key} — either an\n  `authorization: Bearer <token>` header or `authorization: MDTSDB2<key> <signature>`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qomplx/refs/heads/main/authentication/qomplx-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cybersecurity
- Identity Threat Detection
- Managed Detection and Response
- Attack Surface Management
- Time Series
- Analytics
- Risk Management
- Insurance
- Data Platform
---
