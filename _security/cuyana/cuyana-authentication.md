---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cuyana Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cuyana secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cuyana
provider_slug: cuyana
scheme_count: 1
schemes:
- authorizationUrl: https://account.cuyana.com/authentication/oauth/authorize
  endSessionUrl: https://account.cuyana.com/authentication/logout
  flow: authorizationCode
  grantTypes:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  idTokenSigningAlg: RS256
  issuer: https://shopify.com/authentication/71250542907
  jwksUri: https://account.cuyana.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOAuth
  responseTypes:
  - code
  sources:
  - well-known/cuyana-openid-configuration.json
  tokenUrl: https://account.cuyana.com/authentication/oauth/token
  type: oauth2
slug: cuyana-authentication
source_filename: cuyana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cuyana.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Auth surface is Shopify Customer Account OAuth 2.0 / OpenID Connect, discovered via the\n  OIDC + RFC 8414 documents served on cuyana.com. Issuer is Shopify\n  (https://shopify.com/authentication/71250542907); token/authorization endpoints are hosted\n  at account.cuyana.com. This governs customer login and the Customer Account API (including\n  the customer-account-mcp-api scope). PKCE (S256) supported; client auth via client_secret_basic.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  token_endpoint_auth_methods: [client_secret_basic]\nschemes:\n- name: ShopifyCustomerAccountOAuth\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://shopify.com/authentication/71250542907\n  authorizationUrl: https://account.cuyana.com/authentication/oauth/authorize\n\
  \  tokenUrl: https://account.cuyana.com/authentication/oauth/token\n  endSessionUrl: https://account.cuyana.com/authentication/logout\n  jwksUri: https://account.cuyana.com/authentication/.well-known/jwks.json\n  responseTypes: [code]\n  grantTypes:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  idTokenSigningAlg: RS256\n  sources: [well-known/cuyana-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuyana/refs/heads/main/authentication/cuyana-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Fashion
- Retail
- E-commerce
- Direct-to-Consumer
- Apparel
- Leather Goods
- Sustainable Fashion
- Shopify
---
