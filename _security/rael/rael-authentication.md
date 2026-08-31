---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Rael Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rael declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Rael
provider_slug: rael
scheme_count: 2
schemes:
- description: 'tools/list returned HTTP 200 with the full tool manifest on an unauthenticated POST — no WWW-Authenticate header, no OAuth challenge, no invalid_token error. Agents discover and call the catalog surface with no credential. Payment is not authorized by a token: the UCP payment handlers (Google Pay, Shopify card, Shop Pay) require contemporaneous buyer approval at complete_checkout, which is the access control on the write path.'
  evidence:
    auth_challenge: none
    http_status: 200
    probed: '2026-08-26'
  id: mcp-anonymous
  surface: https://www.getrael.com/api/ucp/mcp
  type: none
- description: Shopper sign-in for Rael's store, discovered at /.well-known/openid-configuration on Rael's own domain. Issuer is Shopify, scoped to shop id 22463213. Authorization Code with PKCE (S256), RS256 id_tokens, client_secret_basic/client_secret_post token auth, and a jwt-bearer grant. This is a customer login, not a developer credential — a third party cannot register a client against it from a public page.
  endpoints:
    authorization_endpoint: https://shopify.com/authentication/22463213/oauth/authorize
    end_session_endpoint: https://shopify.com/authentication/22463213/logout
    issuer: https://shopify.com/authentication/22463213
    jwks_uri: https://shopify.com/authentication/22463213/.well-known/jwks.json
    token_endpoint: https://shopify.com/authentication/22463213/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  human_login: https://www.getrael.com/account/login
  id: shopify-customer-accounts
  id_token_signing:
  - RS256
  pkce:
  - S256
  scopes: see scopes/rael-scopes.yml
  surface: https://shopify.com/authentication/22463213
  type: openIdConnect
slug: rael-authentication
source_filename: rael-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.getrael.com/.well-known/openid-configuration + live POST to https://www.getrael.com/api/ucp/mcp\nname: Rael authentication profile\nsummary: >-\n  Rael publishes no developer API keys and runs no developer program. There are exactly two\n  authenticated/anonymous surfaces on its domain, and they are unrelated to each other: the\n  agent commerce MCP endpoint, which is ANONYMOUS, and Shopify Customer Accounts, an OIDC\n  provider for shoppers signing in to their own order history.\nschemes:\n- id: mcp-anonymous\n  surface: https://www.getrael.com/api/ucp/mcp\n  type: none\n  description: >-\n    tools/list returned HTTP 200 with the full tool manifest on an unauthenticated POST — no\n    WWW-Authenticate header, no OAuth challenge, no invalid_token error. Agents discover and\n    call the catalog surface with no credential. Payment is not authorized by a token: the\n    UCP payment handlers (Google Pay, Shopify card,\
  \ Shop Pay) require contemporaneous buyer\n    approval at complete_checkout, which is the access control on the write path.\n  evidence:\n    http_status: 200\n    auth_challenge: none\n    probed: '2026-08-26'\n- id: shopify-customer-accounts\n  surface: https://shopify.com/authentication/22463213\n  type: openIdConnect\n  description: >-\n    Shopper sign-in for Rael's store, discovered at /.well-known/openid-configuration on Rael's\n    own domain. Issuer is Shopify, scoped to shop id 22463213. Authorization Code with PKCE\n    (S256), RS256 id_tokens, client_secret_basic/client_secret_post token auth, and a\n    jwt-bearer grant. This is a customer login, not a developer credential — a third party\n    cannot register a client against it from a public page.\n  endpoints:\n    issuer: https://shopify.com/authentication/22463213\n    authorization_endpoint: https://shopify.com/authentication/22463213/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/22463213/oauth/token\n\
  \    end_session_endpoint: https://shopify.com/authentication/22463213/logout\n    jwks_uri: https://shopify.com/authentication/22463213/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  pkce: [S256]\n  id_token_signing: [RS256]\n  scopes: see scopes/rael-scopes.yml\n  human_login: https://www.getrael.com/account/login\nnot_present:\n- API keys or a key-issuance console\n- A developer portal, app registration, or client credentials flow open to third parties\n- mTLS\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rael/refs/heads/main/authentication/rael-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Health and Wellness
- Personal Care
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
---
