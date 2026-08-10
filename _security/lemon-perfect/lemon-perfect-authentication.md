---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
- agentIdentity
description: ''
kind: authentication
layout: security
method: probed
name: Lemon Perfect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Lemon Perfect secures its APIs with oauth2, openIdConnect, apiKey, and agentIdentity across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Lemon Perfect
provider_slug: lemon-perfect
scheme_count: 4
schemes:
- applies_to: https://lemonperfect.com/api/{version}/graphql.json
  description: Shopify Storefront API public access token. Intended to be embedded in client code — it scopes an app to public storefront data only.
  in: header
  name: StorefrontPublicToken
  observed: Anonymous introspection and anonymous `{shop{name}}` queries both returned HTTP 200 without a token on 2026-08-04, so read access to this surface is effectively open.
  parameter_name: X-Shopify-Storefront-Access-Token
  sources:
  - graphql/lemon-perfect-storefront-2026-07.graphql
  type: apiKey
- authorization_endpoint: https://shopify.com/authentication/3205202020/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  description: Shopify Customer Accounts authorization server bound to this store (shop id 3205202020). Guards the Customer Account API and the customer account MCP API.
  end_session_endpoint: https://shopify.com/authentication/3205202020/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/3205202020
  jwks_uri: https://shopify.com/authentication/3205202020/.well-known/jwks.json
  name: CustomerAccountsOIDC
  openIdConnectUrl: https://lemonperfect.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/lemon-perfect-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/3205202020/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- applies_to: Storefront GraphQL customer* fields and mutations
  description: Legacy Storefront customer access token minted by the `customerAccessTokenCreate` mutation and passed as `customerAccessToken` on customer queries/mutations. Verified present in the 2026-07 SDL.
  name: CustomerAccessToken
  scheme: bearer
  sources:
  - graphql/lemon-perfect-storefront-2026-07.graphql
  type: http
- applies_to: https://lemonperfect.com/api/ucp/mcp
  description: The UCP/MCP endpoint refuses anonymous JSON-RPC calls. The caller must supply a `ucp-agent.profile` URI (mapped to the HTTP UCP-Agent header) resolving to a fetchable platform UCP profile document.
  in: header
  name: UCPAgentProfile
  observed_failure:
    code: invalid_profile_url
    http_status: 422
    jsonrpc_error_code: -32001
    message: 'Unable to fetch agent profile: Missing profile uri'
  parameter_name: UCP-Agent
  sources:
  - mcp/lemon-perfect-mcp.yml
  type: agentIdentity
slug: lemon-perfect-authentication
source_filename: lemon-perfect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://lemonperfect.com/.well-known/openid-configuration\ndocs: https://lemonperfect.com/agents.md\nnote: >-\n  Derived from documents fetched anonymously from lemonperfect.com, not from an\n  OpenAPI securitySchemes block (Lemon Perfect publishes no OpenAPI). Three\n  distinct auth models coexist on the same host: an anonymous/public-token\n  GraphQL storefront, an OIDC-protected customer account authorization server,\n  and an agent-identity gate on the UCP/MCP commerce endpoint.\nsummary:\n  types: [oauth2, openIdConnect, apiKey, agentIdentity]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  pkce: [S256]\nschemes:\n- name: StorefrontPublicToken\n  type: apiKey\n  in: header\n  parameter_name: X-Shopify-Storefront-Access-Token\n  applies_to: https://lemonperfect.com/api/{version}/graphql.json\n  description: >-\n    Shopify Storefront API public access token. Intended to be embedded\
  \ in\n    client code — it scopes an app to public storefront data only.\n  observed: >-\n    Anonymous introspection and anonymous `{shop{name}}` queries both returned\n    HTTP 200 without a token on 2026-08-04, so read access to this surface is\n    effectively open.\n  sources: [graphql/lemon-perfect-storefront-2026-07.graphql]\n- name: CustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://lemonperfect.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/3205202020\n  authorization_endpoint: https://shopify.com/authentication/3205202020/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/3205202020/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/3205202020/logout\n  jwks_uri: https://shopify.com/authentication/3205202020/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported:\
  \ [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  description: >-\n    Shopify Customer Accounts authorization server bound to this store\n    (shop id 3205202020). Guards the Customer Account API and the customer\n    account MCP API.\n  sources: [well-known/lemon-perfect-openid-configuration.json]\n- name: CustomerAccessToken\n  type: http\n  scheme: bearer\n  applies_to: 'Storefront GraphQL customer* fields and mutations'\n  description: >-\n    Legacy Storefront customer access token minted by the\n    `customerAccessTokenCreate` mutation and passed as `customerAccessToken` on\n    customer queries/mutations. Verified present in the 2026-07 SDL.\n  sources: [graphql/lemon-perfect-storefront-2026-07.graphql]\n\
  - name: UCPAgentProfile\n  type: agentIdentity\n  in: header\n  parameter_name: UCP-Agent\n  applies_to: https://lemonperfect.com/api/ucp/mcp\n  description: >-\n    The UCP/MCP endpoint refuses anonymous JSON-RPC calls. The caller must\n    supply a `ucp-agent.profile` URI (mapped to the HTTP UCP-Agent header)\n    resolving to a fetchable platform UCP profile document.\n  observed_failure:\n    http_status: 422\n    jsonrpc_error_code: -32001\n    code: invalid_profile_url\n    message: 'Unable to fetch agent profile: Missing profile uri'\n  sources: [mcp/lemon-perfect-mcp.yml]\nbuyer_consent:\n  required_for: [complete_checkout, payment]\n  policy_url: https://lemonperfect.com/robots.txt\n  description: >-\n    Payment authorization is explicitly reserved to a human. Agents may not\n    finalize a checkout without contemporaneous buyer approval.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - {url: 'https://lemonperfect.com/.well-known/openid-configuration', http_status: 200}\n\
  \  - {url: 'https://lemonperfect.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://lemonperfect.com/api/2026-07/graphql.json', http_status: 200}\n  - {url: 'https://lemonperfect.com/api/ucp/mcp', http_status: 422}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-perfect/refs/heads/main/authentication/lemon-perfect-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/agentIdentity · 4 schemes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Ecommerce
- Retail
- Direct to Consumer
- Agentic Commerce
- Model Context Protocol
- GraphQL
- Universal Commerce Protocol
- Shopify
---
