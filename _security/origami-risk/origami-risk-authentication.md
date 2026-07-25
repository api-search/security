---
api_key_in:
- header
api_specs:
- filename: origami-risk-authentication-openapi.json
  format: json
  label: Origami Risk Authentication API
  slug: origami-risk-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-authentication-openapi.json
- filename: origami-risk-public-api-openapi.json
  format: json
  label: Origami Risk Public API
  slug: origami-risk-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-public-api-openapi.json
- filename: origami-risk-standard-rating-api-openapi.json
  format: json
  label: Origami Risk Standard Rating API
  slug: origami-risk-standard-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-standard-rating-api-openapi.json
auth_types:
- apiKey
- token-endpoint
- hmac
description: Origami Risk authenticates API callers against a provisioned Origami account and client. Two token-request formats are documented against the same credential store (a discrete-field JSON login and an OAuth-shaped client_credentials request), the issued token is then presented on every call in a Token header, and an optional HMAC-SHA1 request-signing scheme is available for callers that need per-call signatures. There is no OpenID Connect discovery document, no authorization-server metadata and no scope surface — the OAuth format is a request shape, not a full OAuth 2.0 authorization server.
kind: authentication
layout: security
method: searched
name: Origami Risk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Origami Risk secures its APIs with apiKey, token-endpoint, and hmac across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Origami Risk
provider_slug: origami-risk
scheme_count: 6
schemes:
- description: The token returned by an Authenticate call, presented on subsequent requests.
  in: header
  name: ApiKeyAuth
  parameter: Token
  sources:
  - openapi/origami-risk-public-api-openapi.json
  - openapi/origami-risk-rating-api-openapi.json
  - https://developers.origamirisk.com/reference/authentication-methods
  type: apiKey
- base_url: https://{environment}.origamirisk.com/OrigamiApi
  docs: https://developers.origamirisk.com/reference/api-token-simple
  endpoint: POST /Authentication/Authenticate
  name: Simple token request
  request_fields:
  - description: The unique identifier for your organization's Origami environment.
    name: Account
    required: true
  - description: The name of the client within the designated Origami Account. Users with cross-client permissions may pass __CrossClientSessionClient to generate a key scoped to all clients the user can access.
    name: ClientName
    required: true
  - description: Your Origami username.
    name: User
    required: true
  - description: The password associated with the User account.
    name: Password
    required: true
  responses:
  - description: OK — token issued
    status: 200
  - description: Unauthorized
    status: 401
  type: token-endpoint
- base_url: https://{environment}.origamirisk.com/OrigamiApi
  docs: https://developers.origamirisk.com/reference/api-token-oauth-format
  endpoint: POST /Authentication/AuthenticateOAuth
  grant_types:
  - client_credentials
  name: OAuth-format token request
  note: client_credentials is the only grant type Origami's APIs support. Client_ID is a composite string "{AccountName}:{ClientName}:{UserName}" and Client_Secret is the password of that user. No scopes are defined and no authorization-server metadata is published, so this is an OAuth-shaped request against the same credential store rather than a conformant OAuth 2.0 authorization server.
  request_fields:
  - default: client_credentials
    name: Grant_Type
    required: true
  - description: '"{AccountName}:{ClientName}:{UserName}" — e.g. AcmeAccount:MunicipleClientPool:AlexanderHamilton'
    name: Client_ID
    required: true
  - description: The password of the {UserName} supplied in Client_ID.
    name: Client_Secret
    required: true
  responses:
  - description: OK — token issued
    status: 200
  - description: Unauthorized
    status: 401
  type: token-endpoint
- algorithm: HMAC-SHA1
  code_samples_published:
  - C#
  - Python
  - PHP
  - Java
  - JavaScript (Node.js)
  - Ruby
  description: Per-call one-way dynamically changing signature. Higher overhead per call, but additional security over a bearer token.
  docs: https://developers.origamirisk.com/reference/hmac-authorization
  encoding: base64
  headers:
  - description: Content type of the call (e.g. application/json). Omitted for GET calls, where it does not apply.
    name: content-type
    required: true
  - description: Request date in the format "yyyy-MM-dd HH:mm:ss zzzz" (e.g. 2018-10-10 22:57:40 -05:00). Requests with a date older than 120 seconds are rejected.
    name: x-api-date
    required: true
  - description: Key identifier string for the calling client application, provided during API setup.
    name: x-api-key
    required: true
  - description: Base64-encoded HMAC-SHA1 hash of the canonical string.
    name: x-api-signature
    required: true
  - description: For API accounts with cross-client access, selects the Client Name for the connection. Not required for single-client accounts.
    name: x-api-clientname
    required: false
  name: HMAC authorization
  replay_window_seconds: 120
  string_to_sign: 'Concatenate with no separators: HTTP method verb (UPPER CASE) + content type (empty string when no content-type header was sent) + request date (matching x-api-date) + request URI path and query without the host (e.g. /OrigamiApi/api/Webhook/GetHandlers) + the secret key issued at API setup. HMAC-SHA1 that input using x-api-key, then base64-encode the result.'
  type: hmac
- docs: https://developers.origamirisk.com/reference/check-if-api-token-has-expired
  endpoint: GET /Authentication/HasTokenExpired
  name: Token expiry check
  note: Confirms whether a previously issued token is still valid.
  type: utility
- docs: https://developers.origamirisk.com/reference/ping
  endpoint: GET /Authentication/Ping
  name: Availability ping
  note: Availability probe published alongside the authentication surface.
  type: utility
slug: origami-risk-authentication
source_filename: origami-risk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://developers.origamirisk.com/reference/authentication-methods\ndocs: https://developers.origamirisk.com/reference/authentication-methods\ndescription: >-\n  Origami Risk authenticates API callers against a provisioned Origami account and\n  client. Two token-request formats are documented against the same credential store\n  (a discrete-field JSON login and an OAuth-shaped client_credentials request), the\n  issued token is then presented on every call in a Token header, and an optional\n  HMAC-SHA1 request-signing scheme is available for callers that need per-call\n  signatures. There is no OpenID Connect discovery document, no authorization-server\n  metadata and no scope surface — the OAuth format is a request shape, not a full\n  OAuth 2.0 authorization server.\nsummary:\n  types:\n  - apiKey\n  - token-endpoint\n  - hmac\n  api_key_in:\n  - header\n  oauth2_flows: []\n  self_serve_credentials: false\n  credential_provisioning:\
  \ >-\n    Credentials require a provisioned Origami Risk account, client and API user.\n    Reading the documentation is self-serve; obtaining a working credential is not.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Token\n  description: The token returned by an Authenticate call, presented on subsequent requests.\n  sources:\n  - openapi/origami-risk-public-api-openapi.json\n  - openapi/origami-risk-rating-api-openapi.json\n  - https://developers.origamirisk.com/reference/authentication-methods\n- name: Simple token request\n  type: token-endpoint\n  endpoint: POST /Authentication/Authenticate\n  base_url: https://{environment}.origamirisk.com/OrigamiApi\n  docs: https://developers.origamirisk.com/reference/api-token-simple\n  request_fields:\n  - name: Account\n    required: true\n    description: The unique identifier for your organization's Origami environment.\n  - name: ClientName\n    required: true\n    description: >-\n      The name of the client\
  \ within the designated Origami Account. Users with\n      cross-client permissions may pass __CrossClientSessionClient to generate a key\n      scoped to all clients the user can access.\n  - name: User\n    required: true\n    description: Your Origami username.\n  - name: Password\n    required: true\n    description: The password associated with the User account.\n  responses:\n  - status: 200\n    description: OK — token issued\n  - status: 401\n    description: Unauthorized\n- name: OAuth-format token request\n  type: token-endpoint\n  endpoint: POST /Authentication/AuthenticateOAuth\n  base_url: https://{environment}.origamirisk.com/OrigamiApi\n  docs: https://developers.origamirisk.com/reference/api-token-oauth-format\n  grant_types:\n  - client_credentials\n  note: >-\n    client_credentials is the only grant type Origami's APIs support. Client_ID is a\n    composite string \"{AccountName}:{ClientName}:{UserName}\" and Client_Secret is the\n    password of that user. No scopes\
  \ are defined and no authorization-server metadata\n    is published, so this is an OAuth-shaped request against the same credential store\n    rather than a conformant OAuth 2.0 authorization server.\n  request_fields:\n  - name: Grant_Type\n    required: true\n    default: client_credentials\n  - name: Client_ID\n    required: true\n    description: '\"{AccountName}:{ClientName}:{UserName}\" — e.g. AcmeAccount:MunicipleClientPool:AlexanderHamilton'\n  - name: Client_Secret\n    required: true\n    description: The password of the {UserName} supplied in Client_ID.\n  responses:\n  - status: 200\n    description: OK — token issued\n  - status: 401\n    description: Unauthorized\n- name: HMAC authorization\n  type: hmac\n  algorithm: HMAC-SHA1\n  encoding: base64\n  docs: https://developers.origamirisk.com/reference/hmac-authorization\n  description: >-\n    Per-call one-way dynamically changing signature. Higher overhead per call, but\n    additional security over a bearer token.\n  headers:\n\
  \  - name: content-type\n    required: true\n    description: >-\n      Content type of the call (e.g. application/json). Omitted for GET calls, where it\n      does not apply.\n  - name: x-api-date\n    required: true\n    description: >-\n      Request date in the format \"yyyy-MM-dd HH:mm:ss zzzz\" (e.g. 2018-10-10 22:57:40\n      -05:00). Requests with a date older than 120 seconds are rejected.\n  - name: x-api-key\n    required: true\n    description: Key identifier string for the calling client application, provided during API setup.\n  - name: x-api-signature\n    required: true\n    description: Base64-encoded HMAC-SHA1 hash of the canonical string.\n  - name: x-api-clientname\n    required: false\n    description: >-\n      For API accounts with cross-client access, selects the Client Name for the\n      connection. Not required for single-client accounts.\n  string_to_sign: >-\n    Concatenate with no separators: HTTP method verb (UPPER CASE) + content type\n    (empty string\
  \ when no content-type header was sent) + request date (matching\n    x-api-date) + request URI path and query without the host (e.g.\n    /OrigamiApi/api/Webhook/GetHandlers) + the secret key issued at API setup. HMAC-SHA1\n    that input using x-api-key, then base64-encode the result.\n  replay_window_seconds: 120\n  code_samples_published:\n  - C#\n  - Python\n  - PHP\n  - Java\n  - JavaScript (Node.js)\n  - Ruby\n- name: Token expiry check\n  type: utility\n  endpoint: GET /Authentication/HasTokenExpired\n  docs: https://developers.origamirisk.com/reference/check-if-api-token-has-expired\n  note: Confirms whether a previously issued token is still valid.\n- name: Availability ping\n  type: utility\n  endpoint: GET /Authentication/Ping\n  docs: https://developers.origamirisk.com/reference/ping\n  note: Availability probe published alongside the authentication surface.\noidc_discovery: false\noauth_authorization_server_metadata: false\nnotes:\n- No /.well-known/openid-configuration or\
  \ /.well-known/oauth-authorization-server is\n  served on any Origami Risk host (probed 2026-07-25, all 404).\n- No OAuth scopes are documented; authorization is governed by the Origami user's\n  configured permissions and client scoping, not by scope strings.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/authentication/origami-risk-authentication.yml
summary_line: apiKey/token-endpoint/hmac · 6 schemes
tags:
- Insurance
- United States
- Property and Casualty
- Policy Administration
- Claims
- Underwriting
- Core Systems
- Risk Management
- Workers Compensation
- Insurtech
- Billing
---
