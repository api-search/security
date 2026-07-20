---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Footway Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Footway secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Footway
provider_slug: footway
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/89171296584/oauth/authorize
  code_challenge_methods_supported:
  - S256
  endSessionEndpoint: https://shopify.com/authentication/89171296584/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/89171296584
  jwksUri: https://shopify.com/authentication/89171296584/.well-known/jwks.json
  name: ShopifyCustomerAccount
  openIdConnectUrl: https://footway.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/footway-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/89171296584/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: footway-authentication
source_filename: footway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://footway.com/.well-known/openid-configuration\ndocs: https://footway.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  note: >-\n    Authenticated customer flows on the footway.com storefront use Shopify\n    Customer Account authentication (OpenID Connect / OAuth 2.0). Read-only\n    catalog/product/collection JSON endpoints require no authentication.\nschemes:\n- name: ShopifyCustomerAccount\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/89171296584\n  openIdConnectUrl: https://footway.com/.well-known/openid-configuration\n  authorizationUrl: https://shopify.com/authentication/89171296584/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/89171296584/oauth/token\n  jwksUri: https://shopify.com/authentication/89171296584/.well-known/jwks.json\n  endSessionEndpoint: https://shopify.com/authentication/89171296584/logout\n\
  \  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources: [well-known/footway-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footway/refs/heads/main/authentication/footway-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- E-commerce
- Marketplace
- Retail
- Footwear
- Fashion
- Shopify
- Agent Commerce
- UCP
- MCP
- Nordic
---
