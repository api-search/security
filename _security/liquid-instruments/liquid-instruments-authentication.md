---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Liquid Instruments Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
- implicit
- password
overview: Liquid Instruments secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, refreshToken, implicit, and password flow(s).
provider_name: Liquid Instruments
provider_slug: liquid-instruments
scheme_count: 3
schemes:
- how_obtained: POST an empty JSON object {} to http://<ip>/api/moku/claim_ownership; the client key is returned in the Moku-Client-Key response header and must be sent on every subsequent request.
  in: header
  name: MokuClientKey
  parameter_name: Moku-Client-Key
  released_by: POST {} to http://<ip>/api/moku/relinquish_ownership
  scope: session — a Moku serves one owner at a time; force_connect / ignore_but overrides exist in the client libraries
  sources:
  - https://apis.liquidinstruments.com/api/getting-started/starting-curl.html
  - pypi:moku 4.3.0.1 moku/session.py (sk_name = "Moku-Client-Key")
  surface: Moku REST API (device-local)
  transport: HTTP (plain) on the local network — the device does not serve TLS
  type: apiKey
- endpoints:
    authorization: https://auth.liquidinstruments.com/oauth2/authorize
    device_authorization: https://auth.liquidinstruments.com/oauth2/device_authorize
    end_session: https://auth.liquidinstruments.com/oauth2/logout
    jwks: https://auth.liquidinstruments.com/.well-known/jwks.json
    token: https://auth.liquidinstruments.com/oauth2/token
    userinfo: https://auth.liquidinstruments.com/oauth2/userinfo
  grant_types_supported:
  - authorization_code
  - password
  - implicit
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - client_credentials
  id_token_signing_alg_values_supported:
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  - RS256
  - RS384
  - RS512
  issuer: https://auth.liquidinstruments.com
  name: LiquidInstrumentsOIDC
  openIdConnectUrl: https://auth.liquidinstruments.com/.well-known/openid-configuration
  pkce: S256 — mokucli login is documented issuing code_challenge + code_challenge_method=S256
  response_modes_supported:
  - form_post
  - fragment
  - query
  response_types_supported:
  - code
  - id_token
  - token id_token
  scopes: see scopes/liquid-instruments-scopes.yml
  sources:
  - https://auth.liquidinstruments.com/.well-known/openid-configuration
  - https://apis.liquidinstruments.com/cli/login.html
  subject_types_supported:
  - public
  surface: Liquid Instruments Identity (hosted)
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: openIdConnect
- description: After interactive OIDC sign-in, `mokucli login` mints a short-lived Security Token Service (STS) credential and caches it locally for subsequent CLI operations. `mokucli logout` clears it.
  name: MokuCLISecurityToken
  scheme: bearer
  sources:
  - https://apis.liquidinstruments.com/cli/login.html
  surface: MokuCLI
  type: http
slug: liquid-instruments-authentication
source_filename: liquid-instruments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://apis.liquidinstruments.com/api/getting-started/starting-curl.html\ndocs:\n- https://apis.liquidinstruments.com/api/getting-started/starting-curl.html\n- https://apis.liquidinstruments.com/cli/login.html\n- https://auth.liquidinstruments.com/.well-known/openid-configuration\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken, implicit, password]\n  note: 'Two distinct authentication surfaces. The device REST API uses a per-session\n    client key minted by the device itself; the hosted cloud services (MokuCLI login,\n    Moku Cloud Compile, licensed features) use OAuth 2.0 / OpenID Connect at\n    auth.liquidinstruments.com. There is no OpenAPI to derive from — this profile was\n    read from the published docs, the OIDC discovery document, and the first-party\n    Python client (PyPI moku 4.3.0.1).'\nschemes:\n-\
  \ name: MokuClientKey\n  surface: Moku REST API (device-local)\n  type: apiKey\n  in: header\n  parameter_name: Moku-Client-Key\n  how_obtained: 'POST an empty JSON object {} to http://<ip>/api/moku/claim_ownership;\n    the client key is returned in the Moku-Client-Key response header and must be sent\n    on every subsequent request.'\n  released_by: 'POST {} to http://<ip>/api/moku/relinquish_ownership'\n  scope: session — a Moku serves one owner at a time; force_connect / ignore_but overrides\n    exist in the client libraries\n  transport: HTTP (plain) on the local network — the device does not serve TLS\n  sources:\n  - https://apis.liquidinstruments.com/api/getting-started/starting-curl.html\n  - 'pypi:moku 4.3.0.1 moku/session.py (sk_name = \"Moku-Client-Key\")'\n- name: LiquidInstrumentsOIDC\n  surface: Liquid Instruments Identity (hosted)\n  type: openIdConnect\n  openIdConnectUrl: https://auth.liquidinstruments.com/.well-known/openid-configuration\n  issuer: https://auth.liquidinstruments.com\n\
  \  endpoints:\n    authorization: https://auth.liquidinstruments.com/oauth2/authorize\n    token: https://auth.liquidinstruments.com/oauth2/token\n    userinfo: https://auth.liquidinstruments.com/oauth2/userinfo\n    device_authorization: https://auth.liquidinstruments.com/oauth2/device_authorize\n    end_session: https://auth.liquidinstruments.com/oauth2/logout\n    jwks: https://auth.liquidinstruments.com/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  - password\n  - implicit\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - client_credentials\n  response_types_supported: [code, id_token, token id_token]\n  response_modes_supported: [form_post, fragment, query]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  id_token_signing_alg_values_supported: [ES256, ES384, ES512, HS256, HS384, HS512, RS256, RS384, RS512]\n  subject_types_supported: [public]\n  pkce: 'S256 — mokucli login is documented\
  \ issuing code_challenge + code_challenge_method=S256'\n  scopes: see scopes/liquid-instruments-scopes.yml\n  sources:\n  - https://auth.liquidinstruments.com/.well-known/openid-configuration\n  - https://apis.liquidinstruments.com/cli/login.html\n- name: MokuCLISecurityToken\n  surface: MokuCLI\n  type: http\n  scheme: bearer\n  description: 'After interactive OIDC sign-in, `mokucli login` mints a short-lived\n    Security Token Service (STS) credential and caches it locally for subsequent CLI\n    operations. `mokucli logout` clears it.'\n  sources:\n  - https://apis.liquidinstruments.com/cli/login.html\ngaps:\n- 'The device REST API is served over plain HTTP on the local network — no TLS, no\n  certificate, no HSTS. The client key is transmitted in clear text on the LAN.'\n- 'No published token lifetime, rotation, or revocation policy for the Moku-Client-Key.'\n- 'The PKCE requirement and the STS token TTL are described in prose, not in a\n  machine-readable security scheme (there is\
  \ no OpenAPI for either surface).'\nx-evidence:\n  fetched: '2026-08-04'\n  openid_configuration_status: 200\n  jwks_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-instruments/refs/heads/main/authentication/liquid-instruments-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Test and Measurement
- Instrumentation
- Hardware
- Oscilloscope
- Spectrum Analyzer
- Data Acquisition
- FPGA
- Photonics
- Scientific Instruments
- Electronics
- Laboratory
---
