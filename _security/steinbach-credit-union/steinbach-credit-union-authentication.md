---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Steinbach Credit Union Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- password
- deviceCode
- ciba
- jwtBearer
- saml2Bearer
- umaTicket
overview: Steinbach Credit Union secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, password, deviceCode, ciba, jwtBearer, saml2Bearer, and umaTicket flow(s).
provider_name: Steinbach Credit Union
provider_slug: steinbach-credit-union
scheme_count: 2
schemes:
- name: openIdConnect
  openIdConnectUrl: https://online.scu.mb.ca/.well-known/openid-configuration
  sources:
  - well-known/steinbach-credit-union-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://online.scu.mb.ca/am/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token
  - flow: clientCredentials
    tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token
  - flow: deviceCode
    note: urn:ietf:params:oauth:grant-type:device_code
  - flow: ciba
    note: urn:openid:params:grant-type:ciba (backchannel authentication)
  name: oauth2
  sources:
  - well-known/steinbach-credit-union-openid-configuration.json
  type: oauth2
slug: steinbach-credit-union-authentication
source_filename: steinbach-credit-union-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://online.scu.mb.ca/.well-known/openid-configuration\ndocs: https://online.scu.mb.ca/am/oauth2\nscope_note: >-\n  This is the CONSUMER / member digital-banking identity provider, not a public\n  developer API. SCU exposes no first-party developer OAuth API. The endpoints\n  below back the online.scu.mb.ca digital banking web/mobile clients (e.g.\n  client_id=InternetBanking) and are operated on a ForgeRock/Ping Access\n  Management OAuth2 authorization server (issuer https://online.scu.mb.ca/am/oauth2).\n  The profile is captured because the OIDC discovery document is anonymously\n  published and is the only machine-readable auth contract SCU exposes.\nsummary:\n  types: [oauth2, openIdConnect]\n  standard: OpenID Connect / OAuth 2.0 (ForgeRock/Ping AM)\n  issuer: https://online.scu.mb.ca/am/oauth2\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, password, deviceCode, ciba, jwtBearer, saml2Bearer, umaTicket]\n\
  \  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt, self_signed_tls_client_auth, tls_client_auth, none]\n  mtls_bound_tokens: true\n  pushed_authorization_requests: available\n  pkce: [S256, plain]\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://online.scu.mb.ca/.well-known/openid-configuration\n  sources: [well-known/steinbach-credit-union-openid-configuration.json]\n- name: oauth2\n  type: oauth2\n  sources: [well-known/steinbach-credit-union-openid-configuration.json]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://online.scu.mb.ca/am/oauth2/authorize\n    tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token\n  - flow: clientCredentials\n    tokenUrl: https://online.scu.mb.ca/am/oauth2/steinbach_token\n  - flow: deviceCode\n    note: urn:ietf:params:oauth:grant-type:device_code\n  - flow: ciba\n    note: urn:openid:params:grant-type:ciba (backchannel authentication)\nendpoints:\n\
  \  authorization: https://online.scu.mb.ca/am/oauth2/authorize\n  token: https://online.scu.mb.ca/am/oauth2/steinbach_token\n  userinfo: https://online.scu.mb.ca/am/oauth2/userinfo\n  introspection: https://online.scu.mb.ca/am/oauth2/introspect\n  revocation: https://online.scu.mb.ca/am/oauth2/token/revoke\n  registration: https://online.scu.mb.ca/am/oauth2/register\n  pushed_authorization_request: https://online.scu.mb.ca/am/oauth2/par\n  end_session: https://online.scu.mb.ca/am/oauth2/connect/endSession\n  jwks_uri: https://online.scu.mb.ca/am/oauth2/connect/jwk_uri\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steinbach-credit-union/refs/heads/main/authentication/steinbach-credit-union-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Manitoba
- Interac
- Data Aggregation
- Open Banking
---
