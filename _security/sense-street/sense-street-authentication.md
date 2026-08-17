---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sense Street Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sense Street secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sense Street
provider_slug: sense-street
scheme_count: 2
schemes:
- algorithm: RS256
  bearerFormat: JWT
  claims:
  - claim: exp
    meaning: expiry
    value: now + 15 minutes
  - claim: nbf
    meaning: not before
    value: now - 5 minutes
  - claim: aud
    meaning: audience
    value: api.sensestreet.com
  - claim: application_id
    meaning: the customer app id issued by Sense Street
  - claim: public_key_id
    default 'default.pub': null
    meaning: identifies which registered public key signed this
  - claim: server_id
    default 'default': null
    meaning: target server identifier
  - claim: server_role
    default 'default': null
    meaning: target server role
  header: Authorization
  in: header
  name: BearerJWT
  not_before_skew_seconds: -300
  scheme: bearer
  source: packages/sense-street-packages.yml
  token_lifetime_seconds: 900
  type: http
  value_format: Bearer <RS256 JWT signed with the client private key>
- description: The client's RSA PUBLIC key is sent verbatim in the X-key header alongside the signed bearer token, so the server can verify the assertion without a prior key exchange for that request. Sending a public key is not a secret disclosure.
  header: X-key
  in: header
  name: XKeyPublicKey
  required: false
  source: packages/sense-street-packages.yml
  type: apiKey
  value_format: PEM-encoded RSA public key
slug: sense-street-authentication
source_filename: sense-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: >-\n  src/sensestreet/auth_header_builder.py in the first-party PyPI package\n  `sensestreet` 1.0.16 (published 2025-10-07), plus the published description of\n  https://docs.sensestreet.com/authentication\ndocs: https://docs.sensestreet.com/authentication\ndocs_gated: true\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  signing_algorithm: RS256\n  key_model: client-held RSA key pair, public key registered with Sense Street\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Sense Street does NOT run OAuth 2.0 or OIDC. There is no authorization\n    server, no /.well-known/openid-configuration, and no scope surface — so this\n    repo carries no scopes/ artifact. Authentication is a client-signed JWT\n    bearer assertion: the customer generates an RSA key pair, registers the\n    public key with Sense Street, and the SDK mints a short-lived RS256 JWT\n    locally for every request. That is a self-issued\
  \ assertion model, not a\n    token-grant model.\nschemes:\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  algorithm: RS256\n  in: header\n  header: Authorization\n  value_format: 'Bearer <RS256 JWT signed with the client private key>'\n  token_lifetime_seconds: 900\n  not_before_skew_seconds: -300\n  claims:\n  - {claim: exp, meaning: expiry, value: now + 15 minutes}\n  - {claim: nbf, meaning: not before, value: now - 5 minutes}\n  - {claim: aud, meaning: audience, value: api.sensestreet.com}\n  - {claim: application_id, meaning: the customer app id issued by Sense Street}\n  - {claim: public_key_id, meaning: identifies which registered public key signed this, default 'default.pub'}\n  - {claim: server_id, meaning: target server identifier, default 'default'}\n  - {claim: server_role, meaning: target server role, default 'default'}\n  source: packages/sense-street-packages.yml\n- name: XKeyPublicKey\n  type: apiKey\n  in: header\n  header: X-key\n  value_format:\
  \ PEM-encoded RSA public key\n  required: false\n  description: >-\n    The client's RSA PUBLIC key is sent verbatim in the X-key header alongside\n    the signed bearer token, so the server can verify the assertion without a\n    prior key exchange for that request. Sending a public key is not a secret\n    disclosure.\n  source: packages/sense-street-packages.yml\nnetwork_controls:\n- control: vpn\n  description: >-\n    \"Enterprise API access is secured with VPN connectivity\" — published on the\n    Sense Street authentication docs page description.\n  source: https://docs.sensestreet.com/authentication\n- control: ip-allowlisting\n  description: >-\n    Static source IPs are allowlisted per customer; the implementation page\n    states integration requires \"secure API integration with static IPs and\n    authentication\".\n  source: https://docs.sensestreet.com/implementation-data-requirements\n- control: edge-auth-gate\n  description: >-\n    Observed live: every path under /api/\
  \ on portal.sensestreet.com returns\n    HTTP 401 with the plain-text body \"Invalid or missing token\", including\n    /api/v1/openapi.json, /api/v1/docs and /api/v1/redoc. The gate is applied at\n    the nginx edge ahead of the application, so unauthenticated callers cannot\n    enumerate the surface.\n  source: probed 2026-08-14\nalways_sent_headers:\n- {header: Authorization, note: only when a private key is configured}\n- {header: X-key, note: PEM public key, only when a public key path is configured}\n- {header: X-client-version, note: SDK version string, e.g. 1.0.16}\n- {header: Date, note: 'client local timestamp, format MM/DD/YYYY, HH:MM:SS'}\n- {header: Content-Type, note: application/json except on multipart file uploads}\ndashboard_authentication:\n  method: sso\n  description: >-\n    The Sense Street dashboard (portal.sensestreet.com) is separate from the API\n    and uses Single Sign-On with role-based access control and MFA. Google\n    Identity Services is loaded on the\
  \ portal login page.\n  source: https://docs.sensestreet.com/dashboard-authentication\nx-evidence:\n- url: https://pypi.org/pypi/sensestreet/json\n  status: 200\n- url: https://docs.sensestreet.com/authentication\n  status: 200\n  note: page renders, body content requires sign-in; the published meta description is the readable part\n- url: https://portal.sensestreet.com/api/v1/ping\n  status: 401\n  note: 'body \"Invalid or missing token\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-street/refs/heads/main/authentication/sense-street-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Capital Markets
- Trading
- Artificial Intelligence
- Fintech
- Conversation Intelligence
- OTC
- Market Data
- Natural Language Processing
- Commodities
- Fixed Income
---
