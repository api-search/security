---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Caliza Authentication
name_suffix: Authentication
oauth_flows:
- password
- authorizationCode
- clientCredentials
overview: Caliza secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, authorizationCode, and clientCredentials flow(s).
provider_name: Caliza
provider_slug: caliza
scheme_count: 1
schemes:
- description: Caliza uses OAuth 2.0 / OpenID Connect backed by Keycloak. The documented quickstart uses the Resource Owner Password Credentials grant (grant_type=password) with a client_id + client_secret (from the dashboard under Settings > API Credentials) plus a username + password. The token response returns an access_token (JWT, ~86400s TTL), a refresh_token, and token_type "Bearer". The Keycloak discovery document additionally advertises authorization_code, client_credentials, refresh_token, implicit, CIBA and device_code grants.
  endpoints:
    authorization: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/auth
    issuer: https://api.caliza.com/auth/realms/caliza
    jwks: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/certs
    sandbox_token: https://api.sandbox.caliza.com/auth/realms/caliza/protocol/openid-connect/token
    token: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
    userinfo: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/userinfo
  flows:
  - documented: true
    flow: password
    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
  - advertised: true
    authorizationUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/auth
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
  - advertised: true
    flow: clientCredentials
    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
  name: OAuth2
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: oauth2
slug: caliza-authentication
source_filename: caliza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.caliza.com/docs/authenticate\ndocs: https://docs.caliza.com/reference/authentication-1\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [password, authorizationCode, clientCredentials]\n  token_transport: bearer\n  identity_provider: Keycloak (realm \"caliza\")\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Caliza uses OAuth 2.0 / OpenID Connect backed by Keycloak. The documented\n    quickstart uses the Resource Owner Password Credentials grant\n    (grant_type=password) with a client_id + client_secret (from the dashboard\n    under Settings > API Credentials) plus a username + password. The token\n    response returns an access_token (JWT, ~86400s TTL), a refresh_token, and\n    token_type \"Bearer\". The Keycloak discovery document additionally advertises\n    authorization_code, client_credentials, refresh_token, implicit, CIBA and\n    device_code grants.\n  flows:\n  - flow:\
  \ password\n    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token\n    documented: true\n  - flow: authorizationCode\n    authorizationUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/auth\n    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token\n    pkce: [S256, plain]\n    advertised: true\n  - flow: clientCredentials\n    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token\n    advertised: true\n  endpoints:\n    issuer: https://api.caliza.com/auth/realms/caliza\n    token: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token\n    authorization: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/auth\n    userinfo: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/userinfo\n    jwks: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/certs\n    sandbox_token: https://api.sandbox.caliza.com/auth/realms/caliza/protocol/openid-connect/token\n\
  \  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\nrequest_authorization:\n  header: Authorization\n  format: 'Bearer {access_token}'\nnotes: >-\n  Every Core API request carries Authorization: Bearer {access_token}. Access\n  tokens are JWTs signed by the Keycloak realm; verify against the jwks endpoint.\n  Realm roles observed in issued tokens include ROLE_INTEGRATOR,\n  ROLE_CREATE_TRANSACTIONS, ROLE_VIEW_ACTIVITY and ROLE_MANAGE_PAYMENT_CONTACTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/authentication/caliza-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Stablecoins
- Remittances
- Foreign Exchange
- Virtual Accounts
- Payouts
- KYC
- Latin America
---
