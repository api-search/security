---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cme Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CME Group secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CME Group
provider_slug: cme-group
scheme_count: 1
schemes:
- authorization_server_metadata:
    authorization_endpoint: https://auth.cmegroup.com/as/authorization.oauth2
    introspection_endpoint: https://auth.cmegroup.com/as/introspect.oauth2
    issuer: https://auth.cmegroup.com
    jwks_uri: https://auth.cmegroup.com/pf/JWKS
    revocation_endpoint: https://auth.cmegroup.com/as/revoke_token.oauth2
    source: well-known/cme-group-oauth-authorization-server.json
    token_endpoint: https://auth.cmegroup.com/as/token.oauth2
  entitlements: Access is entitlement-based per API ID — each API ID must be entitled to the specific API (e.g. Reference Data, FedWatch, Term SOFR) via the CME Group Market Data API self-service onboarding page or Global Account Management. Credentials are environment-specific (New Release vs Production) and cannot be used across environments.
  flows:
  - environment: production
    flow: clientCredentials
    tokenUrl: https://auth.cmegroup.com/as/token.oauth2
  - environment: new-release
    flow: clientCredentials
    tokenUrl: https://authnr.cmegroup.com/as/token.oauth2
  name: CMEGroupOAuth
  token_request:
    authorization: Basic base64(APIID:Password)
    body: grant_type=client_credentials
    content_type: application/x-www-form-urlencoded
    method: POST
  token_response:
    fields:
    - access_token
    - token_type
    - expires_in
    lifetime: about one hour
    token_type: bearer
  type: oauth2
slug: cme-group-authentication
source_filename: cme-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://cmegroupclientsite.atlassian.net/wiki/spaces/EPICSANDBOX/pages/457316022/Client+API+Service+Adoption+Using+OAuth+2.0+Protocol\ndocs: https://cmegroupclientsite.atlassian.net/wiki/spaces/EPICSANDBOX/pages/457316022/Client+API+Service+Adoption+Using+OAuth+2.0+Protocol\nnotes: >-\n  CME Group secures its cloud REST and WebSocket APIs (Reference Data API v3,\n  FedWatch, Term SOFR, Greeks and Implied Volatility, Cross Currency, DataMine)\n  with OAuth 2.0 client-credentials issued against a registered OAuth API ID.\n  API IDs are created in the CME Customer Center under My Profile and must be\n  entitled per API. The authorization server is PingFederate at\n  auth.cmegroup.com and publishes anonymous RFC 8414 / OIDC discovery metadata\n  (captured in well-known/). Legacy Basic Auth API IDs can be irreversibly\n  converted to OAuth IDs. No public OpenAPI declares these schemes — profile\n  captured from the published docs\
  \ and live metadata.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, tls_client_auth]\n  api_request_auth: 'Authorization: Bearer <access_token> (REST GET/POST and WebSocket upgrade)'\nschemes:\n  - name: CMEGroupOAuth\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.cmegroup.com/as/token.oauth2\n        environment: production\n      - flow: clientCredentials\n        tokenUrl: https://authnr.cmegroup.com/as/token.oauth2\n        environment: new-release\n    token_request:\n      method: POST\n      content_type: application/x-www-form-urlencoded\n      authorization: 'Basic base64(APIID:Password)'\n      body: grant_type=client_credentials\n    token_response:\n      fields: [access_token, token_type, expires_in]\n      token_type: bearer\n      lifetime: about one hour\n    authorization_server_metadata:\n      issuer:\
  \ https://auth.cmegroup.com\n      authorization_endpoint: https://auth.cmegroup.com/as/authorization.oauth2\n      token_endpoint: https://auth.cmegroup.com/as/token.oauth2\n      revocation_endpoint: https://auth.cmegroup.com/as/revoke_token.oauth2\n      introspection_endpoint: https://auth.cmegroup.com/as/introspect.oauth2\n      jwks_uri: https://auth.cmegroup.com/pf/JWKS\n      source: well-known/cme-group-oauth-authorization-server.json\n    entitlements: >-\n      Access is entitlement-based per API ID — each API ID must be entitled to\n      the specific API (e.g. Reference Data, FedWatch, Term SOFR) via the CME\n      Group Market Data API self-service onboarding page or Global Account\n      Management. Credentials are environment-specific (New Release vs\n      Production) and cannot be used across environments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cme-group/refs/heads/main/authentication/cme-group-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Capital Markets
- Derivatives
- Exchange
- Financial Markets
- Futures
- Market Data
- Options
- Reference Data
- Trading
- Fortune 1000
---
