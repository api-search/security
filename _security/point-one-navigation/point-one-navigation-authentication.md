---
api_key_in:
- body
auth_types:
- apiKey
- http
- custom
description: ''
kind: authentication
layout: security
method: searched
name: Point One Navigation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Point One Navigation secures its APIs with apiKey, http, and custom across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Point One Navigation
provider_slug: point-one-navigation
scheme_count: 4
schemes:
- api: polaris-native
  description: A Polaris API key (obtained at https://app.pointonenav.com) is POSTed to the token endpoint and exchanged for a short-lived bearer access token used on the corrections stream.
  errors:
  - meaning: FORBIDDEN - invalid API key
    status: 403
  in: body
  name: PolarisApiKeyTokenExchange
  notes:
  - Once connected with a valid token, an established stream keeps receiving data even after the token expires.
  - The access token is presented on the stream in the Authorization system message (class 0xE0, id 0x01) as ASCII.
  parameter: authorization_code
  request:
    authorization_code: <Polaris API key>
    grant_type: authorization_code
    token_type: bearer
    unique_id: <unique connection id>
  response:
    access_token: <token>
    expires_in: '604800'
    issued_at: <timestamp>
    token_type: bearer
  source: https://support.pointonenav.com/native-api-docs
  token_endpoint: https://api.pointonenav.com/api/v1/auth/token
  token_endpoint_auth: none
  token_lifetime_seconds: 604800
  type: apiKey
- api: polaris-ntrip
  description: Exchanges a Polaris API key for a temporary NTRIP username/password pair (~24h) so a fleet can share one key without sharing one credential.
  errors:
  - meaning: FORBIDDEN - invalid API key
    status: 403
  in: body
  name: PolarisNtripDynamicCredentials
  parameter: authorization_code
  source: https://support.pointonenav.com/polaris-ntrip-api-docs
  token_endpoint: https://api.pointonenav.com/api/v1/auth/ntrip
  token_endpoint_auth: none
  token_lifetime_hours: 24
  type: apiKey
- api: polaris-ntrip
  description: Standard NTRIP client authentication against truertk.pointonenav.com. Username must uniquely identify the connection (alphanumeric plus - and _, max 32 chars, no concurrent duplicates); password is issued by Point One or minted via the dynamic-credentials endpoint.
  hosts:
  - host: truertk.pointonenav.com
    port: 2102
    region: north-america
    tls: true
  - host: truertk.pointonenav.com
    port: 2101
    recommended: false
    region: north-america
    tls: false
  - host: truertk-eu.pointonenav.com
    port: 2102
    region: europe
    tls: true
  - host: truertk-eu.pointonenav.com
    port: 2101
    recommended: false
    region: europe
    tls: false
  mountpoints:
  - ITRF2014
  - LOCAL
  name: NtripBasicAuth
  scheme: basic
  source: https://support.pointonenav.com/polaris-ntrip-api-docs
  type: http
- api: graphql
  description: User-scoped Personal Access Token created in the web console under Account > Personal access tokens, with a chosen name, expiration and access level. Shown once at creation and not retrievable afterwards.
  expiration: user-selected at creation
  header:
    captured: false
    reason: The header name/format is documented only on the GraphQL quickstart page at docs.pointonenav.com, which does not render (Docusaurus SPA with undeployed route chunks). Not asserted here rather than guessed.
  managed_by_api: true
  management_operations:
  - viewPersonalAccessTokens
  - createPersonalAccessToken
  - revokePersonalAccessToken
  - deletePersonalAccessToken
  name: PersonalAccessToken
  roles:
  - grants:
    - query
    - subscription
    role: read-only
  - grants:
    - query
    - subscription
    - mutation
    role: read/write
  source: https://support.pointonenav.com/graphql-api-personal-access-token
  type: apiKey
slug: point-one-navigation-authentication
source_filename: point-one-navigation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://support.pointonenav.com/native-api-docs\ndocs:\n- https://support.pointonenav.com/native-api-docs\n- https://support.pointonenav.com/polaris-ntrip-api-docs\n- https://support.pointonenav.com/graphql-api-personal-access-token\nsummary:\n  types: [apiKey, http, custom]\n  api_key_in: [body]\n  oauth2_flows: []\n  note: >-\n    Point One does not run an OAuth 2.0 authorization server. The Polaris services use a bearer-token\n    exchange that borrows OAuth vocabulary (grant_type / token_type / access_token) over a single\n    unauthenticated POST, and the platform GraphQL API uses long-lived Personal Access Tokens minted\n    in the web console. There is no /.well-known/oauth-authorization-server and no\n    /.well-known/openid-configuration on any host (all probed 404 or SPA catch-all).\nschemes:\n- name: PolarisApiKeyTokenExchange\n  type: apiKey\n  in: body\n  parameter: authorization_code\n  api: polaris-native\n \
  \ description: >-\n    A Polaris API key (obtained at https://app.pointonenav.com) is POSTed to the token endpoint and\n    exchanged for a short-lived bearer access token used on the corrections stream.\n  token_endpoint: https://api.pointonenav.com/api/v1/auth/token\n  token_endpoint_auth: none\n  request:\n    grant_type: authorization_code\n    token_type: bearer\n    authorization_code: '<Polaris API key>'\n    unique_id: '<unique connection id>'\n  response:\n    token_type: bearer\n    access_token: '<token>'\n    expires_in: '604800'\n    issued_at: '<timestamp>'\n  token_lifetime_seconds: 604800\n  errors:\n  - {status: 403, meaning: FORBIDDEN - invalid API key}\n  notes:\n  - Once connected with a valid token, an established stream keeps receiving data even after the token expires.\n  - The access token is presented on the stream in the Authorization system message (class 0xE0, id 0x01) as ASCII.\n  source: https://support.pointonenav.com/native-api-docs\n- name: PolarisNtripDynamicCredentials\n\
  \  type: apiKey\n  in: body\n  parameter: authorization_code\n  api: polaris-ntrip\n  description: >-\n    Exchanges a Polaris API key for a temporary NTRIP username/password pair (~24h) so a fleet can\n    share one key without sharing one credential.\n  token_endpoint: https://api.pointonenav.com/api/v1/auth/ntrip\n  token_endpoint_auth: none\n  token_lifetime_hours: 24\n  errors:\n  - {status: 403, meaning: FORBIDDEN - invalid API key}\n  source: https://support.pointonenav.com/polaris-ntrip-api-docs\n- name: NtripBasicAuth\n  type: http\n  scheme: basic\n  api: polaris-ntrip\n  description: >-\n    Standard NTRIP client authentication against truertk.pointonenav.com. Username must uniquely\n    identify the connection (alphanumeric plus - and _, max 32 chars, no concurrent duplicates);\n    password is issued by Point One or minted via the dynamic-credentials endpoint.\n  hosts:\n  - {host: truertk.pointonenav.com, port: 2102, tls: true, region: north-america}\n  - {host: truertk.pointonenav.com,\
  \ port: 2101, tls: false, region: north-america, recommended: false}\n  - {host: truertk-eu.pointonenav.com, port: 2102, tls: true, region: europe}\n  - {host: truertk-eu.pointonenav.com, port: 2101, tls: false, region: europe, recommended: false}\n  mountpoints: [ITRF2014, LOCAL]\n  source: https://support.pointonenav.com/polaris-ntrip-api-docs\n- name: PersonalAccessToken\n  type: apiKey\n  api: graphql\n  description: >-\n    User-scoped Personal Access Token created in the web console under Account > Personal access\n    tokens, with a chosen name, expiration and access level. Shown once at creation and not\n    retrievable afterwards.\n  roles:\n  - {role: read-only, grants: [query, subscription]}\n  - {role: read/write, grants: [query, subscription, mutation]}\n  managed_by_api: true\n  management_operations: [viewPersonalAccessTokens, createPersonalAccessToken, revokePersonalAccessToken, deletePersonalAccessToken]\n  expiration: user-selected at creation\n  header:\n    captured:\
  \ false\n    reason: >-\n      The header name/format is documented only on the GraphQL quickstart page at\n      docs.pointonenav.com, which does not render (Docusaurus SPA with undeployed route chunks).\n      Not asserted here rather than guessed.\n  source: https://support.pointonenav.com/graphql-api-personal-access-token\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://api.pointonenav.com/api/v1/auth/ntrip', method: GET, http_status: 405, note: 'HTTP 405 confirms the endpoint exists and is POST-only'}\n  - {url: 'https://graphql.pointonenav.com/graphql', method: POST, http_status: 401, note: 'UNAUTHENTICATED - token required'}\n  - {url: 'https://api.pointonenav.com/.well-known/openid-configuration', http_status: 404}\n  - {url: 'https://api.pointonenav.com/.well-known/oauth-authorization-server', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/point-one-navigation/refs/heads/main/authentication/point-one-navigation-authentication.yml
summary_line: apiKey/http/custom · 4 schemes
tags:
- Location
- GNSS
- Positioning
- Geospatial
- RTK
- Navigation
- Mapping
- Robotics
- Autonomous Vehicles
- IoT
- Hardware
- GraphQL
---
