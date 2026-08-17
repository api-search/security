---
api_key_in:
- header
api_specs:
- filename: franklin-whole-home-openapi.yml
  format: yaml
  label: FranklinWH API
  slug: franklinwh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/openapi/franklin-whole-home-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Franklin Whole Home Authentication
name_suffix: Authentication
oauth_flows: []
overview: Franklin Whole Home secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Franklin Whole Home
provider_slug: franklin-whole-home
scheme_count: 1
schemes:
- description: Token returned by POST /api-common/tokenizer (exchange of a `cp` / `ck` credential pair). Sent as the raw Authorization header value with no `Bearer ` prefix.
  in: header
  name: AuthorizationToken
  parameter: Authorization
  sources:
  - openapi/franklin-whole-home-openapi.yml
  type: apiKey
slug: franklin-whole-home-authentication
source_filename: franklin-whole-home-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: openapi/franklin-whole-home-openapi.yml\ndocs: https://api.franklinwh.com/\nreferences:\n- https://api.franklinwh.com/\n- https://www.franklinwh.com/blog/introducing-the-franklinwh-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: credential-pair exchanged for an opaque token\nschemes:\n- name: AuthorizationToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token returned by POST /api-common/tokenizer (exchange of a `cp` / `ck` credential\n    pair). Sent as the raw Authorization header value with no `Bearer ` prefix.\n  sources:\n  - openapi/franklin-whole-home-openapi.yml\ntoken_issuance:\n  operation: tokenizer\n  method: POST\n  path: /api-common/tokenizer\n  credentials:\n  - name: cp\n    required: true\n    note: Credential pair identifier issued to the partner.\n  - name: ck\n    required: true\n    note: Credential pair key issued to the partner.\n\
  \  security: none\n  note: The token endpoint is the only unauthenticated operation in the API.\n  lifetime: not published\n  refresh: Re-call the same operation; the portal labels it \"Update Token\".\nfailure_modes:\n- code: 401\n  http_status: 200\n  msg: wrong token\n  note: Token present but invalid or expired. Returned inside a HTTP 200 body.\n- code: 403\n  http_status: 200\n  msg: missing token or token param\n  note: Token absent, or cp/ck omitted on the token request. Returned inside a HTTP 200 body.\nonboarding:\n  model: partner-approval\n  sso: FleetView single sign-on — installers sign in with an existing FleetView account\n    (https://energy.franklinwh.com/) and the API portal applies the associated device scope,\n    avoiding a duplicate account.\n  audience: Authorised partners only — third-party system owners and financiers, large and midsize\n    installers, and third-party service providers.\n  url: https://www.franklinwh.com/apply?role=installer\nscopes:\n  model:\
  \ implicit\n  note: >-\n    No OAuth 2.0 and no scope surface. FranklinWH states the API offers \"flexible, granular\n    permission controls\" and that the portal applies the device scope attached to the FleetView\n    account, but publishes no scope, permission or role vocabulary — access is bound to the\n    credential pair rather than requested per call. scopes/ is therefore not emitted.\ntransport_security:\n  tls_claim: TLS 1.3\n  tls_observed: TLSv1.3\n  observed_hosts:\n  - test-api.franklinwh.com\n  - api.franklinwh.com\n  key_storage_claim: FranklinWH states API keys are stored as hashes rather than plaintext.\n  source: https://www.franklinwh.com/blog/introducing-the-franklinwh-api\ngaps:\n- No published token lifetime, expiry semantics or refresh policy.\n- No OIDC or OAuth 2.0 metadata — /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server return 404 on every host.\n- Authentication and authorisation failures are signalled inside a HTTP 200 body,\
  \ so standard HTTP\n  client auth handling will not fire.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/franklin-whole-home/refs/heads/main/authentication/franklin-whole-home-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Energy
- Energy Storage
- Home Energy Management
- Solar
- Batteries
- Internet of Things
- Smart Home
- Electric Vehicles
- Cleantech
- Device Telemetry
---
