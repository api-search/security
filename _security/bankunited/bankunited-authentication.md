---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bankunited Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: BankUnited secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: BankUnited
provider_slug: bankunited
scheme_count: 2
schemes:
- issuer: https://developer.bankunited.com/aeh
  name: OpenIDConnect
  openIdConnectUrl: https://developer.bankunited.com/aeh/.well-known/openid-configuration
  sources:
  - well-known/bankunited-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.bankunited.com/aeh/services/oauth2/token
  - authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize
    flow: implicit
  introspectionUrl: https://developer.bankunited.com/aeh/services/oauth2/introspect
  jwksUri: https://developer.bankunited.com/aeh/id/keys
  name: OAuth2
  registrationUrl: https://developer.bankunited.com/aeh/services/oauth2/register
  revocationUrl: https://developer.bankunited.com/aeh/services/oauth2/revoke
  sources:
  - well-known/bankunited-openid-configuration.json
  type: oauth2
  userinfoUrl: https://developer.bankunited.com/aeh/services/oauth2/userinfo
slug: bankunited-authentication
source_filename: bankunited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.bankunited.com/aeh/.well-known/openid-configuration\ndocs: https://developer.bankunited.com/s/\nnotes: >-\n  Derived from the anonymously-published OpenID Connect discovery document of the\n  BankUnited API Experience Hub developer portal. The portal is a Salesforce\n  Experience Cloud site, so the auth surface is Salesforce's OAuth 2.0 / OpenID\n  Connect implementation: authorization code and implicit (token / id_token)\n  response types, RS256-signed ID tokens, token revocation, introspection,\n  userinfo and dynamic client registration endpoints. Developers register an app\n  in the portal to obtain client credentials; the specific product API scopes and\n  contracts are behind portal login. Client authentication supports\n  client_secret_post, client_secret_basic and private_key_jwt.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit]\n  token_endpoint_auth_methods:\
  \ [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg: [RS256]\n  pkce: unknown\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://developer.bankunited.com/aeh/.well-known/openid-configuration\n  issuer: https://developer.bankunited.com/aeh\n  sources: [well-known/bankunited-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize\n    tokenUrl: https://developer.bankunited.com/aeh/services/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://developer.bankunited.com/aeh/services/oauth2/authorize\n  revocationUrl: https://developer.bankunited.com/aeh/services/oauth2/revoke\n  introspectionUrl: https://developer.bankunited.com/aeh/services/oauth2/introspect\n  userinfoUrl: https://developer.bankunited.com/aeh/services/oauth2/userinfo\n  registrationUrl: https://developer.bankunited.com/aeh/services/oauth2/register\n\
  \  jwksUri: https://developer.bankunited.com/aeh/id/keys\n  sources: [well-known/bankunited-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankunited/refs/heads/main/authentication/bankunited-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Commercial Banking
- Open Finance
- Developer Portal
---
