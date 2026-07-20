---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Italist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Italist secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Italist
provider_slug: italist
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/70535250059/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/70535250059
  jwks_uri: https://shopify.com/authentication/70535250059/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://italist.com/.well-known/openid-configuration
  response_types:
  - code
  token_endpoint: https://shopify.com/authentication/70535250059/oauth/token
  type: openIdConnect
slug: italist-authentication
source_filename: italist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://italist.com/.well-known/openid-configuration\nnote: >-\n  italist.com is a Shopify storefront. Buyer/customer authentication is handled by\n  Shopify's Customer Account API via OpenID Connect (issuer shopify.com). Agentic\n  commerce over the UCP/MCP endpoint requires buyer-approved payment; read-only\n  product/collection browsing requires no authentication.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://italist.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/70535250059\n  authorization_endpoint: https://shopify.com/authentication/70535250059/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/70535250059/oauth/token\n  jwks_uri: https://shopify.com/authentication/70535250059/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  id_token_signing_alg: RS256\n  code_challenge_methods:\n  - S256\nunauthenticated_surfaces:\n- description: Read-only storefront product/collection JSON (no auth)\n  examples:\n  - GET /products/{handle}.json\n  - GET /collections/{handle}/products.json\n  - GET /collections/all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/italist/refs/heads/main/authentication/italist-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- E-commerce
- Retail
- Fashion
- Luxury
- Marketplace
- Shopify
- Agentic Commerce
- MCP
---
