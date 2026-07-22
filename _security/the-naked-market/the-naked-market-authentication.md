---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Naked Market Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Naked Market declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: The Naked Market
provider_slug: the-naked-market
scheme_count: 3
schemes:
- authorization_endpoint: https://shopify.com/authentication/52367163575/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/52367163575/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_algs:
  - RS256
  issuer: https://shopify.com/authentication/52367163575
  jwks_uri: https://shopify.com/authentication/52367163575/.well-known/jwks.json
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/52367163575/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- description: UCP MCP endpoint (POST /api/ucp/mcp) requires agent identification via a UCP-Agent profile URI (meta.ucp-agent.profile / UCP-Agent header) per the Universal Commerce Protocol; checkout completion additionally requires explicit buyer approval.
  id: ucp-agent-profile
  type: http
- description: Product and collection JSON endpoints and search require no authentication.
  id: anonymous-storefront-read
  type: none
slug: the-naked-market-authentication
source_filename: the-naked-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thenakedmarket.com/.well-known/openid-configuration (live fetch, HTTP 200)\nname: The Naked Market authentication profile\nnotes: >-\n  The Naked Market is a Shopify-hosted storefront; customer authentication is provided by\n  Shopify Customer Accounts via OpenID Connect. The store publishes both\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server on its own\n  domain. The agent-commerce (UCP/MCP) surface separately requires a UCP-Agent profile URI on\n  each request; storefront read endpoints (/products/{handle}.json,\n  /collections/{handle}/products.json) are unauthenticated.\nschemes:\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/52367163575\n  authorization_endpoint: https://shopify.com/authentication/52367163575/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/52367163575/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/52367163575/logout\n  jwks_uri: https://shopify.com/authentication/52367163575/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_algs:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n- id: ucp-agent-profile\n  type: http\n  description: >-\n    UCP MCP endpoint (POST /api/ucp/mcp) requires agent identification via a UCP-Agent profile\n    URI (meta.ucp-agent.profile / UCP-Agent header) per the Universal Commerce Protocol;\n    checkout completion additionally requires explicit buyer approval.\n- id: anonymous-storefront-read\n  type: none\n  description: Product and collection JSON endpoints and search require no authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-naked-market/refs/heads/main/authentication/the-naked-market-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Consumer
- Consumer Packaged Goods
- Food and Beverage
- Direct to Consumer
- Snacks
- Brand Incubator
- E-Commerce
---
