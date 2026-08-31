---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Poppi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Poppi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Poppi
provider_slug: poppi
scheme_count: 2
schemes:
- applies_to: https://drinkpoppi.com/api/ucp/mcp
  description: The UCP MCP endpoint accepts unauthenticated JSON-RPC. No Authorization header was sent and tools/list returned HTTP 200 with the full tool manifest. Payment is gated by buyer approval at complete_checkout, not by an API credential.
  id: none
  type: none
  verified: probed
- applies_to: https://shopify.com/authentication/22399731
  authorization_endpoint: https://shopify.com/authentication/22399731/oauth/authorize
  description: Shopify Customer Accounts OIDC for the poppi store (issuer https://shopify.com/authentication/22399731, shop 22399731). Login entry point is https://drinkpoppi.com/account/login, which 302s into this tenant.
  end_session_endpoint: https://shopify.com/authentication/22399731/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: oidc-customer-accounts
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/22399731/.well-known/jwks.json
  openIdConnectUrl: https://drinkpoppi.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/22399731/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
slug: poppi-authentication
source_filename: poppi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://drinkpoppi.com/.well-known/openid-configuration,\n  https://drinkpoppi.com/.well-known/oauth-authorization-server,\n  https://drinkpoppi.com/api/ucp/mcp (anonymous tools/list, HTTP 200),\n  https://drinkpoppi.com/agents.md\nnote: >-\n  poppi publishes no developer program and no API keys. There are two distinct auth surfaces, and they are\n  not the same product: the agent commerce MCP endpoint is ANONYMOUS (tools/list returned 200 with no\n  credential), while customer accounts on the storefront run OAuth 2.0 / OpenID Connect against the store's\n  own Shopify Customer Accounts tenant. Both were probed directly, not inferred from docs.\nschemes:\n- id: none\n  type: none\n  applies_to: https://drinkpoppi.com/api/ucp/mcp\n  description: >-\n    The UCP MCP endpoint accepts unauthenticated JSON-RPC. No Authorization header was sent and tools/list\n    returned HTTP 200 with the full tool manifest. Payment is gated\
  \ by buyer approval at\n    complete_checkout, not by an API credential.\n  verified: probed\n- id: oidc-customer-accounts\n  type: openIdConnect\n  applies_to: https://shopify.com/authentication/22399731\n  openIdConnectUrl: https://drinkpoppi.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/22399731/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/22399731/oauth/token\n  jwks_uri: https://shopify.com/authentication/22399731/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/22399731/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg: [RS256]\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  description: >-\n    Shopify Customer\
  \ Accounts OIDC for the poppi store (issuer https://shopify.com/authentication/22399731,\n    shop 22399731). Login entry point is https://drinkpoppi.com/account/login, which 302s into this tenant.\n  verified: probed\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppi/refs/heads/main/authentication/poppi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Consumer Packaged Goods
- Beverages
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- MCP
---
