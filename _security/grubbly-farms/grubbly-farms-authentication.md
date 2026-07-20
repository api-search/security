---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Grubbly Farms Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Grubbly Farms secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Grubbly Farms
provider_slug: grubbly-farms
scheme_count: 2
schemes:
- issuer: https://shopify.com/authentication/14073744
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://grubblyfarms.com/.well-known/openid-configuration
  sources:
  - well-known/grubbly-farms-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://account.grubblyfarms.com/authentication/oauth/authorize
    codeChallengeMethod: S256
    flow: authorizationCode
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://account.grubblyfarms.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  jwks_uri: https://account.grubblyfarms.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oauth2
  sources:
  - well-known/grubbly-farms-oauth-authorization-server.json
  type: oauth2
slug: grubbly-farms-authentication
source_filename: grubbly-farms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://grubblyfarms.com/.well-known/openid-configuration\ndocs: https://account.grubblyfarms.com/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  notes: >-\n    Grubbly Farms authenticates customers through the Shopify Customer Account identity\n    surface, advertised via OpenID Connect / OAuth 2.0 Authorization Server Metadata\n    (RFC 8414) discovery documents. Authorization-code flow with PKCE (S256). This governs\n    customer-account and customer-account-mcp API access; the anonymous Storefront MCP\n    server at /api/mcp does not require a user token for public catalog/cart operations.\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://grubblyfarms.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/14073744\n\
  \  sources: [well-known/grubbly-farms-openid-configuration.json]\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.grubblyfarms.com/authentication/oauth/authorize\n    tokenUrl: https://account.grubblyfarms.com/authentication/oauth/token\n    codeChallengeMethod: S256\n    scopes:\n    - openid\n    - email\n    - customer-account-api:full\n    - customer-account-mcp-api:full\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  jwks_uri: https://account.grubblyfarms.com/authentication/.well-known/jwks.json\n  sources: [well-known/grubbly-farms-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubbly-farms/refs/heads/main/authentication/grubbly-farms-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- E-Commerce
- Retail
- Consumer Packaged Goods
- Pet & Animal
- Poultry
- Sustainability
- Shopify
- MCP
- Agentic Commerce
---
