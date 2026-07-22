---
api_key_in: []
auth_types: []
description: Authenticated buyer and agent actions against Winc's Shopify-hosted store use the Shopify Customer Account API, secured with OpenID Connect / OAuth 2.0 (authorization code + PKCE). Read-only catalog browsing over the storefront and UCP catalog tools is unauthenticated.
kind: authentication
layout: security
method: searched
name: Winc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Winc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Winc
provider_slug: winc
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/77589545277/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/77589545277/logout
  flows:
  - authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/77589545277
  jwks_uri: https://shopify.com/authentication/77589545277/.well-known/jwks.json
  openid_connect_url: https://winc.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/77589545277/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: winc-authentication
source_filename: winc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://winc.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nname: Winc Authentication Profile\ndescription: >-\n  Authenticated buyer and agent actions against Winc's Shopify-hosted store use the Shopify\n  Customer Account API, secured with OpenID Connect / OAuth 2.0 (authorization code + PKCE).\n  Read-only catalog browsing over the storefront and UCP catalog tools is unauthenticated.\nprovider: Shopify Customer Account API\nschemes:\n- id: shopify_customer_account_oidc\n  type: openIdConnect\n  flows:\n  - authorization_code\n  openid_connect_url: https://winc.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/77589545277\n  authorization_endpoint: https://shopify.com/authentication/77589545277/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/77589545277/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/77589545277/logout\n\
  \  jwks_uri: https://shopify.com/authentication/77589545277/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\nunauthenticated_surface:\n- Storefront product/collection JSON (GET /products/{handle}.json, /collections/{handle}/products.json)\n- Storefront search (GET /search?q=...&type=product)\n- UCP catalog search/lookup and cart creation prior to buyer-approved checkout\nnotes:\n- Payment completion always requires explicit buyer approval (see llms.txt / UCP checkout rules).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/winc/refs/heads/main/authentication/winc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Wine
- Ecommerce
- Retail
- Subscription
- Agentic Commerce
- MCP
- Shopify
- UCP
---
