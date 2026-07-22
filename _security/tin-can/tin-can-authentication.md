---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tin Can Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tin Can secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tin Can
provider_slug: tin-can
scheme_count: 1
schemes:
- authorizationUrl: https://manage.tincan.kids/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/89002967405
  jwks_uri: https://manage.tincan.kids/authentication/.well-known/jwks.json
  name: shopifyCustomerAccounts
  openIdConnectUrl: https://tincan.kids/.well-known/openid-configuration
  scope_count: 4
  sources:
  - well-known/tin-can-openid-configuration.json
  tokenUrl: https://manage.tincan.kids/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: tin-can-authentication
source_filename: tin-can-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/tin-can-openid-configuration.json + live probe of\n  https://tincan.kids/api/mcp (2026-07-21)\ndocs: null\nnotes: >-\n  Tin Can publishes no first-party developer API. Its authenticated surface is\n  the Shopify Customer Accounts OIDC/OAuth 2.0 authorization server served on\n  the provider's own domain (manage.tincan.kids). The Shopify storefront MCP\n  endpoint (https://tincan.kids/api/mcp) answered tools/list without\n  authentication.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  unauthenticated_surfaces: [storefront MCP catalog/cart tools, storefront\n      product/collection JSON endpoints]\nschemes:\n- name: shopifyCustomerAccounts\n  type: openIdConnect\n  openIdConnectUrl: https://tincan.kids/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/89002967405\n  authorizationUrl: https://manage.tincan.kids/authentication/oauth/authorize\n\
  \  tokenUrl: https://manage.tincan.kids/authentication/oauth/token\n  jwks_uri: https://manage.tincan.kids/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scope_count: 4\n  sources: [well-known/tin-can-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tin-can/refs/heads/main/authentication/tin-can-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Hardware
- Telecommunications
- Voice
- Kids
- Phones
---
