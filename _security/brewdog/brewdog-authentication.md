---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- none
description: ''
kind: authentication
layout: security
method: probed
name: Brewdog Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BrewDog secures its APIs with openIdConnect, oauth2, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BrewDog
provider_slug: brewdog
scheme_count: 3
schemes:
- applies_to: BrewDog customer accounts (https://brewdog.com/account)
  authorizationUrl: https://shopify.com/authentication/82272813382/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  endSessionUrl: https://shopify.com/authentication/82272813382/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_algs:
  - RS256
  issuer: https://shopify.com/authentication/82272813382
  jwksUri: https://shopify.com/authentication/82272813382/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://brewdog.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/brewdog-openid-configuration.json
  subject_types:
  - public
  tokenUrl: https://shopify.com/authentication/82272813382/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to: https://brewdog.com/api/ucp/mcp
  description: The UCP MCP endpoint does not accept anonymous JSON-RPC. An unauthenticated tools/list returns HTTP 422 with JSON-RPC error -32001 "UCP discovery failed" (data.code = invalid_profile_url, "Missing profile uri"), so the caller must present a resolvable agent profile URI before any tool is listed or invoked.
  name: ucp-agent-profile
  payment_authorization: Completing a checkout additionally requires contemporaneous buyer approval; the payment handlers are Google Pay, Shopify Card and Shop Pay.
  scheme: UCP agent profile URI
  sources:
  - mcp/brewdog-mcp.yml
  type: agent-identity
- applies_to: https://brewdog.com/products.json, /products/{handle}.json, /collections/{handle}/products.json, /search?q={query}&type=product
  description: BrewDog documents its read-only storefront product/collection JSON endpoints for agents as requiring no authentication. Verified with an anonymous GET (HTTP 200, application/json).
  name: none
  sources:
  - llms/brewdog-agents.md
  type: none
slug: brewdog-authentication
source_filename: brewdog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://brewdog.com/.well-known/openid-configuration\ndocs: https://brewdog.com/agents.md\nnote: BrewDog publishes no OpenAPI, so this profile is not derived from securitySchemes.\n  It is read from the OIDC/OAuth discovery documents BrewDog serves from its own\n  origin, plus the authentication behaviour observed on each live surface.\nsummary:\n  types: [openIdConnect, oauth2, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  unauthenticated_surfaces: 2\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://brewdog.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/82272813382\n  authorizationUrl: https://shopify.com/authentication/82272813382/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/82272813382/oauth/token\n  endSessionUrl: https://shopify.com/authentication/82272813382/logout\n  jwksUri: https://shopify.com/authentication/82272813382/.well-known/jwks.json\n\
  \  response_types: [code]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_algs: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/brewdog-openid-configuration.json]\n  applies_to: BrewDog customer accounts (https://brewdog.com/account)\n- name: ucp-agent-profile\n  type: agent-identity\n  scheme: UCP agent profile URI\n  sources: [mcp/brewdog-mcp.yml]\n  applies_to: https://brewdog.com/api/ucp/mcp\n  description: The UCP MCP endpoint does not accept anonymous JSON-RPC. An unauthenticated\n    tools/list returns HTTP 422 with JSON-RPC error -32001 \"UCP discovery failed\"\n    (data.code = invalid_profile_url, \"Missing profile uri\"), so the caller must\n    present a resolvable\
  \ agent profile URI before any tool is listed or invoked.\n  payment_authorization: Completing a checkout additionally requires contemporaneous\n    buyer approval; the payment handlers are Google Pay, Shopify Card and Shop Pay.\n- name: none\n  type: none\n  sources: [llms/brewdog-agents.md]\n  applies_to: https://brewdog.com/products.json, /products/{handle}.json,\n    /collections/{handle}/products.json, /search?q={query}&type=product\n  description: BrewDog documents its read-only storefront product/collection JSON\n    endpoints for agents as requiring no authentication. Verified with an anonymous\n    GET (HTTP 200, application/json).\nx-evidence:\n  fetched: '2026-08-02'\n  probes:\n  - url: https://brewdog.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json; charset=utf-8\n  - url: https://brewdog.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json; charset=utf-8\n  - url: https://brewdog.com/api/ucp/mcp\n\
  \    http_status: 422\n    note: anonymous tools/list rejected\n  - url: https://brewdog.com/products.json?limit=2\n    http_status: 200\n    note: anonymous read succeeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brewdog/refs/heads/main/authentication/brewdog-authentication.yml
summary_line: openIdConnect/oauth2/none · 3 schemes
tags:
- Company
- Food and Beverage
- Beer
- Brewing
- Retail
- E-Commerce
- Consumer Packaged Goods
- Hospitality
- Agentic Commerce
- Shopify
---
