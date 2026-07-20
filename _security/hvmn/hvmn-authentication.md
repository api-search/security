---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hvmn Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HVMN secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HVMN
provider_slug: hvmn
scheme_count: 1
schemes:
- authorizationUrl: https://account.ketone.com/authentication/oauth/authorize
  codeChallengeMethods:
  - S256
  endSessionUrl: https://account.ketone.com/authentication/logout
  grantTypes:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  idTokenSigningAlg:
  - RS256
  issuer: https://shopify.com/authentication/25727336499
  jwksUri: https://account.ketone.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://ketone.com/.well-known/openid-configuration
  responseTypes:
  - code
  sources:
  - well-known/hvmn-openid-configuration.json
  tokenEndpointAuthMethods:
  - client_secret_basic
  tokenUrl: https://account.ketone.com/authentication/oauth/token
  type: openIdConnect
slug: hvmn-authentication
source_filename: hvmn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://ketone.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: >-\n    Authentication is Shopify Customer Account (OAuth 2.0 + OpenID Connect).\n    The store publishes OIDC discovery at /.well-known/openid-configuration and\n    RFC 8414 authorization-server metadata at /.well-known/oauth-authorization-server.\n    Storefront read endpoints (products.json, collections, search) require no\n    authentication; the UCP MCP commerce endpoint transacts under buyer approval.\nschemes:\n  - name: ShopifyCustomerAccount\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/25727336499\n    openIdConnectUrl: https://ketone.com/.well-known/openid-configuration\n    authorizationUrl: https://account.ketone.com/authentication/oauth/authorize\n    tokenUrl: https://account.ketone.com/authentication/oauth/token\n\
  \    endSessionUrl: https://account.ketone.com/authentication/logout\n    jwksUri: https://account.ketone.com/authentication/.well-known/jwks.json\n    responseTypes: [code]\n    grantTypes:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenEndpointAuthMethods: [client_secret_basic]\n    codeChallengeMethods: [S256]\n    idTokenSigningAlg: [RS256]\n    sources: [well-known/hvmn-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hvmn/refs/heads/main/authentication/hvmn-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Health
- Nutrition
- Ketones
- Supplements
- E-Commerce
- Shopify
- Agentic Commerce
- Consumer
- MCP
---
