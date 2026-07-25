---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Pico Trading Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Pico secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Pico
provider_slug: pico-trading
scheme_count: 2
schemes:
- issuer: https://portal.pico.net
  name: portalOIDC
  openIdConnectUrl: https://portal.pico.net/.well-known/openid-configuration
  scope: Customer portal login (Salesforce Experience Cloud), not a public product-API scheme.
  sources:
  - well-known/pico-trading-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://portal.pico.net/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://portal.pico.net/services/oauth2/token
  introspectionUrl: https://portal.pico.net/services/oauth2/introspect
  name: portalOAuth2
  registrationUrl: https://portal.pico.net/services/oauth2/register
  revocationUrl: https://portal.pico.net/services/oauth2/revoke
  sources:
  - well-known/pico-trading-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
slug: pico-trading-authentication
source_filename: pico-trading-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://portal.pico.net/.well-known/openid-configuration\ndocs: https://portal.pico.net/\nnote: Pico publishes no public API reference, so no product-API security\n  schemes can be derived. The only publicly documented authentication surface\n  is the login-gated Salesforce Experience Cloud customer portal\n  (portal.pico.net) that fronts all product and Corvil API documentation; its\n  OAuth 2.0 / OpenID Connect configuration is published via OIDC discovery.\n  Authentication to the product APIs themselves (Corvil REST API/SDK, Redline\n  InRush embedded API, RedlineFeed multicast entitlements) is\n  entitlement-managed and documented only behind the customer portal.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: portalOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://portal.pico.net/.well-known/openid-configuration\n  issuer: https://portal.pico.net\n\
  \  scope: Customer portal login (Salesforce Experience Cloud), not a public\n    product-API scheme.\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n- name: portalOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.pico.net/services/oauth2/authorize\n    tokenUrl: https://portal.pico.net/services/oauth2/token\n  revocationUrl: https://portal.pico.net/services/oauth2/revoke\n  introspectionUrl: https://portal.pico.net/services/oauth2/introspect\n  registrationUrl: https://portal.pico.net/services/oauth2/register\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  sources:\n  - well-known/pico-trading-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico-trading/refs/heads/main/authentication/pico-trading-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Market Data
- Trading
- Real-Time
- Low Latency
- Feed Handlers
- Order Execution
- Network Analytics
- Exchange Connectivity
---
