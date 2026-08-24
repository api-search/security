---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hint declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hint
provider_slug: hint
scheme_count: 2
schemes:
- applies_to: https://www.drinkhint.com/api/ucp/mcp
  description: tools/list and the catalog tools answer unauthenticated. Rejection observed on 2026-08-22 was for a MISSING meta.ucp-agent.profile (JSON-RPC -32001 invalid_profile_url, HTTP 422), not for a missing credential.
  evidence: anonymous POST tools/list returned HTTP 200 with 13 tools
  id: mcp_anonymous
  type: none
- applies_to: storefront customer account (login, orders, subscriptions)
  authorization_endpoint: https://shopify.com/authentication/1430159418/oauth/authorize
  bearer_methods_supported:
  - header
  end_session_endpoint: https://shopify.com/authentication/1430159418/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  human_entry_point: https://www.drinkhint.com/account/login
  id: shopify_customer_accounts_oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/1430159418
  jwks_uri: https://shopify.com/authentication/1430159418/.well-known/jwks.json
  openIdConnectUrl: https://www.drinkhint.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  protected_resource: https://www.drinkhint.com
  response_types:
  - code
  token_endpoint: https://shopify.com/authentication/1430159418/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: hint-authentication
source_filename: hint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://www.drinkhint.com/.well-known/openid-configuration,\n  https://www.drinkhint.com/.well-known/oauth-protected-resource,\n  and an anonymous JSON-RPC tools/list against https://www.drinkhint.com/api/ucp/mcp\nsummary: >-\n  Two distinct auth postures. The agentic commerce surface (UCP/MCP) is ANONYMOUS — catalog, cart\n  and checkout tools answered without any credential; the only required call context is a\n  meta.ucp-agent.profile URI, which identifies the agent rather than authenticating it, and payment\n  is gated on contemporaneous human approval rather than on a token. Buyer accounts use Shopify\n  Customer Accounts, an OpenID Connect provider with authorization code + PKCE.\nschemes:\n- id: mcp_anonymous\n  type: none\n  applies_to: https://www.drinkhint.com/api/ucp/mcp\n  description: >-\n    tools/list and the catalog tools answer unauthenticated. Rejection observed on 2026-08-22 was\n    for a MISSING meta.ucp-agent.profile\
  \ (JSON-RPC -32001 invalid_profile_url, HTTP 422), not for a\n    missing credential.\n  evidence: anonymous POST tools/list returned HTTP 200 with 13 tools\n- id: shopify_customer_accounts_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.drinkhint.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/1430159418\n  authorization_endpoint: https://shopify.com/authentication/1430159418/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/1430159418/oauth/token\n  jwks_uri: https://shopify.com/authentication/1430159418/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/1430159418/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n\
  \  bearer_methods_supported:\n  - header\n  protected_resource: https://www.drinkhint.com\n  applies_to: storefront customer account (login, orders, subscriptions)\n  human_entry_point: https://www.drinkhint.com/account/login\nnotes:\n- No API keys, no developer application registration, and no partner program are published by Hint.\n- The OIDC provider is Shopify's, scoped to this merchant's shop id (1430159418); Hint does not run\n  its own identity provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint/refs/heads/main/authentication/hint-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Ecommerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
---
