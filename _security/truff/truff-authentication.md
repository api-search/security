---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Truff Authentication
name_suffix: Authentication
oauth_flows: []
overview: TRUFF declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TRUFF
provider_slug: truff
scheme_count: 3
schemes:
- applies_to: https://shop.truff.com/api/ucp/mcp
  evidence: Unauthenticated POST returned HTTP 200 with 13 tools and their inputSchemas; no 401, no WWW-Authenticate header, no oauth-protected-resource metadata.
  id: none
  note: 'Caller identity is asserted rather than authenticated: every tool requires meta.ucp-agent.profile, a URI naming the calling agent. That is attribution, not authentication.'
  type: none
- applies_to: https://shop.truff.com/products.json, /products/{handle}.json, /collections/{handle}/products.json, /search?q=&type=product
  evidence: GET https://shop.truff.com/products.json?limit=3 returned HTTP 200 application/json. llms.txt documents these under "Read-Only Browsing (No Authentication Required)".
  id: none-storefront-json
  type: none
- applies_to: storefront shopper accounts (not the API surface)
  authorization_endpoint: https://shopify.com/authentication/21822603/oauth/authorize
  evidence: Served at https://shop.truff.com/.well-known/openid-configuration and https://truff.com/.well-known/openid-configuration, HTTP 200.
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_alg: RS256
  issuer: https://shopify.com/authentication/21822603
  jwks_uri: https://shopify.com/authentication/21822603/.well-known/jwks.json
  note: Platform-provided. The issuer is Shopify's per-shop identity service; TRUFF does not operate it and publishes no client-registration path for it.
  pkce: S256
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/21822603/oauth/token
  type: openIdConnect
slug: truff-authentication
source_filename: truff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  POST https://shop.truff.com/api/ucp/mcp tools/list (HTTP 200, no credentials sent) and\n  GET https://shop.truff.com/.well-known/openid-configuration (HTTP 200), probed 2026-08-30.\ndocs: https://shop.truff.com/llms.txt\nsummary: >-\n  TRUFF's agent-facing commerce surface is anonymous. The UCP MCP endpoint answered a full\n  tools/list with no Authorization header, no API key and no OAuth challenge, and the\n  published agent instructions describe the read-only storefront JSON endpoints as requiring\n  no authentication. There is no API-key issuance, no developer registration and no developer\n  OAuth application flow anywhere on TRUFF's hosts. The one identity surface that exists is\n  Shopify's hosted Customer Accounts OIDC provider, which authenticates SHOPPERS to the\n  storefront — it is not a developer credential.\nschemes:\n- id: none\n  type: none\n  applies_to: https://shop.truff.com/api/ucp/mcp\n  evidence: >-\n\
  \    Unauthenticated POST returned HTTP 200 with 13 tools and their inputSchemas; no 401, no\n    WWW-Authenticate header, no oauth-protected-resource metadata.\n  note: >-\n    Caller identity is asserted rather than authenticated: every tool requires\n    meta.ucp-agent.profile, a URI naming the calling agent. That is attribution, not\n    authentication.\n- id: none-storefront-json\n  type: none\n  applies_to: >-\n    https://shop.truff.com/products.json, /products/{handle}.json,\n    /collections/{handle}/products.json, /search?q=&type=product\n  evidence: >-\n    GET https://shop.truff.com/products.json?limit=3 returned HTTP 200 application/json.\n    llms.txt documents these under \"Read-Only Browsing (No Authentication Required)\".\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  applies_to: storefront shopper accounts (not the API surface)\n  issuer: https://shopify.com/authentication/21822603\n  authorization_endpoint: https://shopify.com/authentication/21822603/oauth/authorize\n\
  \  token_endpoint: https://shopify.com/authentication/21822603/oauth/token\n  jwks_uri: https://shopify.com/authentication/21822603/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: S256\n  id_token_alg: RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  evidence: >-\n    Served at https://shop.truff.com/.well-known/openid-configuration and\n    https://truff.com/.well-known/openid-configuration, HTTP 200.\n  note: >-\n    Platform-provided. The issuer is Shopify's per-shop identity service; TRUFF does not\n    operate it and publishes no client-registration path for it.\npayment_credentials:\n  note: >-\n    Payment is handled by declared UCP payment handlers (Google Pay, Shopify Card, Shop Pay).\n    Agents never handle raw card credentials; complete_checkout takes a tokenized instrument\n    and requires contemporaneous buyer approval.\ngaps:\n- No\
  \ developer API keys are issued and no developer portal exists.\n- No /.well-known/oauth-protected-resource is served for the MCP endpoint.\n- No security.txt on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truff/refs/heads/main/authentication/truff-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Condiments
- Direct to Consumer
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Shopify
---
