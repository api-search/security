---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nasdaq Private Market Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
- refreshToken
overview: Nasdaq Private Market secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Nasdaq Private Market
provider_slug: nasdaq-private-market
scheme_count: 2
schemes:
- endpoints:
    authorization: https://fe.login.secondmarket.com/oauth2/v1/authorize
    introspection: https://fe.login.secondmarket.com/oauth2/v1/introspect
    jwks: https://fe.login.secondmarket.com/oauth2/v1/keys
    registration: https://fe.login.secondmarket.com/oauth2/v1/clients
    revocation: https://fe.login.secondmarket.com/oauth2/v1/revoke
    token: https://fe.login.secondmarket.com/oauth2/v1/token
    userinfo: https://fe.login.secondmarket.com/oauth2/v1/userinfo
  id_token_signing_alg:
  - RS256
  issuer: https://fe.login.secondmarket.com
  name: NPM Platform OIDC (Okta)
  openIdConnectUrl: https://fe.login.secondmarket.com/.well-known/openid-configuration
  response_types:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  sources:
  - well-known/nasdaq-private-market-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  issuer: https://fe.login.secondmarket.com
  metadata: https://fe.login.secondmarket.com/.well-known/oauth-authorization-server
  name: NPM Platform OAuth 2.0 Authorization Server
  sources:
  - well-known/nasdaq-private-market-oauth-authorization-server.json
  type: oauth2
slug: nasdaq-private-market-authentication
source_filename: nasdaq-private-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://fe.login.secondmarket.com/.well-known/openid-configuration\ndocs: https://www.nasdaqprivatemarket.com/data-intelligence/\nnotes: 'Nasdaq Private Market publishes no OpenAPI and no developer authentication\n  documentation. This profile is derived entirely from the live OpenID Connect / RFC\n  8414 discovery documents served by the platform identity host, plus the published\n  access tiers on the Data & Intelligence page. It describes how a human signs in to\n  the NPM / SecondMarket trading platform — it is NOT a documented machine-to-machine\n  contract for the Tape D data API, which is sold on the Premium (Talk to Sales) tier\n  and delivered through Nasdaq Data Link.'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  pkce: true\n  pkce_methods:\n  - S256\n  dynamic_client_registration:\
  \ true\nschemes:\n- name: NPM Platform OIDC (Okta)\n  type: openIdConnect\n  openIdConnectUrl: https://fe.login.secondmarket.com/.well-known/openid-configuration\n  issuer: https://fe.login.secondmarket.com\n  endpoints:\n    authorization: https://fe.login.secondmarket.com/oauth2/v1/authorize\n    token: https://fe.login.secondmarket.com/oauth2/v1/token\n    userinfo: https://fe.login.secondmarket.com/oauth2/v1/userinfo\n    jwks: https://fe.login.secondmarket.com/oauth2/v1/keys\n    registration: https://fe.login.secondmarket.com/oauth2/v1/clients\n    introspection: https://fe.login.secondmarket.com/oauth2/v1/introspect\n    revocation: https://fe.login.secondmarket.com/oauth2/v1/revoke\n  id_token_signing_alg:\n  - RS256\n  response_types:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  sources:\n\
  \  - well-known/nasdaq-private-market-openid-configuration.json\n- name: NPM Platform OAuth 2.0 Authorization Server\n  type: oauth2\n  metadata: https://fe.login.secondmarket.com/.well-known/oauth-authorization-server\n  issuer: https://fe.login.secondmarket.com\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  sources:\n  - well-known/nasdaq-private-market-oauth-authorization-server.json\ngaps:\n- No public API authentication guide — the \"Learn about API Access\" link on the Data\n  & Intelligence page is an empty \"#\" anchor.\n- No API key / token provisioning surface is documented for the Tape D dataset; the\n  only published path is \"Talk to Sales\" for the Premium tier.\n- No scope reference for the data products; the scopes advertised by the identity host\n  are identity/profile scopes and Okta org-management scopes, not NPM\
  \ business scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-private-market/refs/heads/main/authentication/nasdaq-private-market-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Private Markets
- Secondary Markets
- Market Data
- Financial-Services
- Valuations
- Pre-IPO Equity
- Capital Markets
---
