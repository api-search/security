---
api_key_in: []
auth_types: []
description: Supergoop! has no developer program and issues no API keys. Its machine surfaces authenticate in three distinct ways, all observed live on 2026-08-29.
kind: authentication
layout: security
method: probed
name: Supergoop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supergoop! declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Supergoop!
provider_slug: supergoop
scheme_count: 5
schemes:
- applies_to:
  - https://supergoop.com/api/2026-07/graphql.json (catalog, collections, blog, pages, cart)
  - https://supergoop.com/products.json
  - https://supergoop.com/collections/{handle}/products.json
  - POST https://supergoop.com/api/ucp/mcp method=tools/list
  evidence: Full GraphQL introspection and a products query both returned HTTP 200 with no Authorization header and no X-Shopify-Storefront-Access-Token.
  id: anonymous-public-read
  type: none
- applies_to:
  - POST https://supergoop.com/api/ucp/mcp tools/call (catalog + cart + checkout tools)
  description: Every UCP tool call carries a `meta.ucp-agent.profile` URI identifying the calling agent. The server FETCHES that URI; an unreachable profile is rejected with JSON-RPC error -32001 / profile_unreachable and HTTP 422. This is identity-by-published-document rather than a bearer credential.
  evidence: examples/supergoop-ucp-mcp-error-profile-unreachable.json
  id: ucp-agent-profile
  location: request body (JSON-RPC params.arguments.meta)
  parameter: meta['ucp-agent'].profile
  required: true
  type: agent-profile
- applies_to:
  - POST https://supergoop.com/api/ucp/mcp tools/call name=get_order
  description: Order-scoped tools require a JWT. An anonymous call returned HTTP 403 with JSON-RPC error -32000 AuthenticationRequired and a pointer to https://shopify.dev/docs/agents/get-started/authentication.
  evidence: examples/supergoop-ucp-mcp-error-authentication-required.json
  format: JWT
  id: ucp-jwt
  required: true
  scheme: bearer
  type: http
- applies_to:
  - https://supergoop.com/account (shopper sign-in)
  - Customer Account API / customer-account-mcp-api
  authorization_endpoint: https://shopify.com/authentication/15035658/oauth/authorize
  description: Shopper identity for supergoop.com is an OIDC provider hosted by Shopify on behalf of this store (shop id 15035658). The discovery documents are served from supergoop.com; the issuer and endpoints are on shopify.com.
  end_session_endpoint: https://shopify.com/authentication/15035658/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/15035658
  jwks_uri: https://shopify.com/authentication/15035658/.well-known/jwks.json
  openIdConnectUrl: https://supergoop.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/15035658/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to:
  - Storefront GraphQL customer{} field and customer* mutations
  description: Customer-scoped Storefront GraphQL fields take a customer access token minted by Mutation.customerAccessTokenCreate. Present in the live schema; not exercised.
  id: storefront-customer-access-token
  location: header
  name: X-Shopify-Customer-Access-Token
  type: apiKey
slug: supergoop-authentication
source_filename: supergoop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://supergoop.com/.well-known/oauth-authorization-server ;\n  https://supergoop.com/.well-known/oauth-protected-resource ;\n  https://supergoop.com/api/ucp/mcp ; https://supergoop.com/api/2026-07/graphql.json\ndescription: >-\n  Supergoop! has no developer program and issues no API keys. Its machine\n  surfaces authenticate in three distinct ways, all observed live on 2026-08-29.\nschemes:\n  - id: anonymous-public-read\n    type: none\n    applies_to:\n      - https://supergoop.com/api/2026-07/graphql.json (catalog, collections, blog, pages, cart)\n      - https://supergoop.com/products.json\n      - https://supergoop.com/collections/{handle}/products.json\n      - 'POST https://supergoop.com/api/ucp/mcp method=tools/list'\n    evidence: >-\n      Full GraphQL introspection and a products query both returned HTTP 200 with\n      no Authorization header and no X-Shopify-Storefront-Access-Token.\n  - id: ucp-agent-profile\n\
  \    type: agent-profile\n    applies_to:\n      - 'POST https://supergoop.com/api/ucp/mcp tools/call (catalog + cart + checkout tools)'\n    parameter: meta['ucp-agent'].profile\n    location: request body (JSON-RPC params.arguments.meta)\n    required: true\n    description: >-\n      Every UCP tool call carries a `meta.ucp-agent.profile` URI identifying the\n      calling agent. The server FETCHES that URI; an unreachable profile is\n      rejected with JSON-RPC error -32001 / profile_unreachable and HTTP 422. This\n      is identity-by-published-document rather than a bearer credential.\n    evidence: examples/supergoop-ucp-mcp-error-profile-unreachable.json\n  - id: ucp-jwt\n    type: http\n    scheme: bearer\n    format: JWT\n    applies_to:\n      - 'POST https://supergoop.com/api/ucp/mcp tools/call name=get_order'\n    required: true\n    description: >-\n      Order-scoped tools require a JWT. An anonymous call returned HTTP 403 with\n      JSON-RPC error -32000 AuthenticationRequired\
  \ and a pointer to\n      https://shopify.dev/docs/agents/get-started/authentication.\n    evidence: examples/supergoop-ucp-mcp-error-authentication-required.json\n  - id: shopify-customer-accounts-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://supergoop.com/.well-known/openid-configuration\n    applies_to:\n      - https://supergoop.com/account (shopper sign-in)\n      - Customer Account API / customer-account-mcp-api\n    issuer: https://shopify.com/authentication/15035658\n    authorization_endpoint: https://shopify.com/authentication/15035658/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/15035658/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/15035658/logout\n    jwks_uri: https://shopify.com/authentication/15035658/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types: [code]\n    pkce: [S256]\n    token_endpoint_auth_methods:\
  \ [client_secret_basic, client_secret_post]\n    id_token_signing_alg: [RS256]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    description: >-\n      Shopper identity for supergoop.com is an OIDC provider hosted by Shopify on\n      behalf of this store (shop id 15035658). The discovery documents are served\n      from supergoop.com; the issuer and endpoints are on shopify.com.\n  - id: storefront-customer-access-token\n    type: apiKey\n    name: X-Shopify-Customer-Access-Token\n    location: header\n    applies_to:\n      - Storefront GraphQL customer{} field and customer* mutations\n    description: >-\n      Customer-scoped Storefront GraphQL fields take a customer access token\n      minted by Mutation.customerAccessTokenCreate. Present in the live schema;\n      not exercised.\nnotes:\n  - No API keys, client credentials, or partner registration are offered by Supergoop! itself.\n  - >-\n    No developer portal exists. The authentication\
  \ surface is entirely the\n    Shopify commerce platform's, exposed on Supergoop!'s domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supergoop/refs/heads/main/authentication/supergoop-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Sunscreen
- Skincare
- Beauty
- Cosmetics
- Consumer Goods
- Retail
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
---
