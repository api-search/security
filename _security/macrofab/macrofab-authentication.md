---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Macrofab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MacroFab secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MacroFab
provider_slug: macrofab
scheme_count: 2
schemes:
- issuer: https://factory.macrofab.com
  name: OpenIDConnect
  openIdConnectUrl: https://factory.macrofab.com/.well-known/openid-configuration
  sources:
  - well-known/macrofab-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://factory.macrofab.com/oauth/authorize
    flow: authorizationCode
    scopes:
      email: Access to the account email address
      openid: OpenID Connect authentication
    tokenUrl: https://factory.macrofab.com/oauth/token
  id_token_signing_alg_values_supported:
  - RS256
  jwks_uri: https://factory.macrofab.com/oauth/jwks.json
  name: OAuth2
  response_types_supported:
  - code
  sources:
  - well-known/macrofab-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: macrofab-authentication
source_filename: macrofab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://factory.macrofab.com/.well-known/openid-configuration\ndocs: https://support.macrofab.com\nnotes: >-\n  Derived from MacroFab's live OpenID Connect discovery document on the customer\n  manufacturing platform (factory.macrofab.com). MacroFab does not publish an open\n  OpenAPI/Swagger definition; the platform is authenticated. The OIDC metadata below\n  is the authoritative, provider-published auth contract for the factory platform.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  scopes: [openid, email]\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://factory.macrofab.com/.well-known/openid-configuration\n    issuer: https://factory.macrofab.com\n    sources: [well-known/macrofab-openid-configuration.json]\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://factory.macrofab.com/oauth/authorize\n\
  \        tokenUrl: https://factory.macrofab.com/oauth/token\n        scopes:\n          openid: OpenID Connect authentication\n          email: Access to the account email address\n    jwks_uri: https://factory.macrofab.com/oauth/jwks.json\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    id_token_signing_alg_values_supported: [RS256]\n    response_types_supported: [code]\n    sources: [well-known/macrofab-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrofab/refs/heads/main/authentication/macrofab-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Hardware
- Electronics Manufacturing
- PCB Assembly
- Contract Manufacturing
- Supply Chain
- Manufacturing AI
- ITAR
---
