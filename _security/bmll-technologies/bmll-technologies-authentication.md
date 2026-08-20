---
api_key_in:
- header
auth_types:
- key-pair-jwt
- bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bmll Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: BMLL Technologies secures its APIs with key-pair-jwt, bearer, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BMLL Technologies
provider_slug: bmll-technologies
scheme_count: 3
schemes:
- credentials:
    passphrase: BMLL_KEY_PASSPHRASE env var (optional)
    private_key: BMLL_KEY_PATH env var (path to PEM private key; public key must sit next to it as .pub)
    username: BMLL_USERNAME env var (api username / email; may also be read from the public key comment field)
  description: Two-step handshake against the auth service. Step 1 POST /auth/identity with {iss = username} returns a session id (sid). Step 2 sends signed-JWT claims {iss = username, aud, exp (24h), sid} — signed with the user's PEM private key (optionally passphrase-protected) — to obtain a bearer token. Audience is "dd-services" for the data-plane auth service and "lab-services" for the Data Lab lab-auth service.
  endpoints:
    auth: https://auth.data.bmlltech.com
    lab_auth: https://auth.lab.bmlltech.com
  name: key-pair-jwt
  type: custom
- description: 'The token obtained from the handshake is sent as an "Authorization: Bearer <token>" header on all service requests.'
  name: bearer
  scheme: bearer
  type: http
- description: Data Lab (lab-auth) logins additionally fetch an API key from the account service (GET /api-key) and send it as the x-api-key header.
  in: header
  name: x-api-key
  parameter: x-api-key
  type: apiKey
slug: bmll-technologies-authentication
source_filename: bmll-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: bmll Python SDK 1.24.7 source (bmll/_rest.py), https://pypi.org/project/bmll/\ndocs: https://pypi.org/project/bmll/\nsummary:\n  types: [key-pair-jwt, bearer, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  self_serve: false\n  note: No OAuth2/OIDC. Access is sales-led with per-account entitlements; no\n    public signup or self-serve API keys.\nmodel: |\n  Authentication is key-pair based. A user registers at\n  https://data.bmlltech.com (sales-provisioned) and generates an SSH-style\n  key-pair. The SDK signs a JWT with the PEM private key and exchanges it in a\n  two-step handshake with the auth service, then sends the resulting token as\n  a Bearer header on every data-plane request (plus an x-api-key header for\n  Data Lab flows).\nschemes:\n- name: key-pair-jwt\n  type: custom\n  description: Two-step handshake against the auth service. Step 1 POST\n    /auth/identity with {iss = username} returns a session id\
  \ (sid). Step 2\n    sends signed-JWT claims {iss = username, aud, exp (24h), sid} — signed with\n    the user's PEM private key (optionally passphrase-protected) — to obtain a\n    bearer token. Audience is \"dd-services\" for the data-plane auth service and\n    \"lab-services\" for the Data Lab lab-auth service.\n  credentials:\n    username: BMLL_USERNAME env var (api username / email; may also be read from\n      the public key comment field)\n    private_key: BMLL_KEY_PATH env var (path to PEM private key; public key must\n      sit next to it as .pub)\n    passphrase: BMLL_KEY_PASSPHRASE env var (optional)\n  endpoints:\n    auth: https://auth.data.bmlltech.com\n    lab_auth: https://auth.lab.bmlltech.com\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'The token obtained from the handshake is sent as an\n    \"Authorization: Bearer <token>\" header on all service requests.'\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description:\
  \ Data Lab (lab-auth) logins additionally fetch an API key from the\n    account service (GET /api-key) and send it as the x-api-key header.\nheaders:\n  version: x-bmll-version (SDK version) is sent on every request.\nbehavior:\n  reauth_on_401: The SDK re-logins once on a 401 and retries; a second\n    consecutive 401 raises AuthenticationError.\n  entitlements: Per-account entitlements gate which datasets/services a token\n    can access; quota is inspected at https://data.bmlltech.com/#app/permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmll-technologies/refs/heads/main/authentication/bmll-technologies-authentication.yml
summary_line: key-pair-jwt/bearer/apiKey · 3 schemes
tags:
- Financial
- Market Data
- Order Book
- Stocks
- Trading
- Reference Data
- Historical Data
- Analytics
- ETFs
- Futures
- Options
---
