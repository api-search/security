---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Wrogn (USPL / Universal Sportsbiz) Shopify storefront, captured from live discovery documents on wrogn.com. There is no separate developer program: the machine surface is the Shopify-native storefront (product JSON, storefront MCP, UCP), with customer identity via Shopify Customer Accounts OIDC published on the store''s own host.'
kind: authentication
layout: security
method: searched
name: Uspl Wrogn Authentication
name_suffix: Authentication
oauth_flows: []
overview: USPL Wrogn declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: USPL Wrogn
provider_slug: uspl-wrogn
scheme_count: 3
schemes:
- authorization_endpoint: https://shopify.com/authentication/81803051309/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/81803051309
  jwks_uri: https://shopify.com/authentication/81803051309/.well-known/jwks.json
  name: customer-accounts-oidc
  openIdConnectUrl: https://wrogn.com/.well-known/openid-configuration
  pkce: S256
  response_types:
  - code
  scopes: scopes/uspl-wrogn-scopes.yml
  token_endpoint: https://shopify.com/authentication/81803051309/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- description: 'Read-only storefront browsing and the storefront MCP catalog/cart tools require no authentication: GET /products/{handle}.json, GET /collections/{handle}/products.json, GET /search?q=, and POST /api/mcp (tools/list answered unauthenticated at probe time, 2026-07-21). Rate-limited per IP.'
  name: anonymous-storefront
  type: none
- description: The UCP MCP endpoint (POST /api/ucp/mcp) requires a Universal Commerce Protocol agent profile; without one it returns JSON-RPC -32001 invalid_profile_url. Discovery at https://wrogn.com/.well-known/ucp.
  name: ucp-agent-profile
  type: other
slug: uspl-wrogn-authentication
source_filename: uspl-wrogn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://wrogn.com/.well-known/openid-configuration\ndescription: >-\n  Authentication profile for the Wrogn (USPL / Universal Sportsbiz) Shopify\n  storefront, captured from live discovery documents on wrogn.com. There is\n  no separate developer program: the machine surface is the Shopify-native\n  storefront (product JSON, storefront MCP, UCP), with customer identity via\n  Shopify Customer Accounts OIDC published on the store's own host.\nschemes:\n  - name: customer-accounts-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://wrogn.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/81803051309\n    authorization_endpoint: https://shopify.com/authentication/81803051309/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/81803051309/oauth/token\n    jwks_uri: https://shopify.com/authentication/81803051309/.well-known/jwks.json\n    response_types: [code]\n   \
  \ pkce: S256\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    token_endpoint_auth_methods: [client_secret_basic]\n    id_token_signing_alg: RS256\n    scopes: scopes/uspl-wrogn-scopes.yml\n  - name: anonymous-storefront\n    type: none\n    description: >-\n      Read-only storefront browsing and the storefront MCP catalog/cart tools\n      require no authentication: GET /products/{handle}.json,\n      GET /collections/{handle}/products.json, GET /search?q=, and\n      POST /api/mcp (tools/list answered unauthenticated at probe time,\n      2026-07-21). Rate-limited per IP.\n  - name: ucp-agent-profile\n    type: other\n    description: >-\n      The UCP MCP endpoint (POST /api/ucp/mcp) requires a Universal Commerce\n      Protocol agent profile; without one it returns JSON-RPC -32001\n      invalid_profile_url. Discovery at https://wrogn.com/.well-known/ucp.\nnotes:\n  - Customer login at https://wrogn.com/account/login\
  \ (Shopify Customer Accounts).\n  - No API-key or developer-token scheme is published by the brand.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspl-wrogn/refs/heads/main/authentication/uspl-wrogn-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Consumer
- Fashion
- Apparel
- eCommerce
- Retail
- India
- Agentic Commerce
- MCP
---
