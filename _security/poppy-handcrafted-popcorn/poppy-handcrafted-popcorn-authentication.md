---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Poppy Handcrafted Popcorn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Poppy Handcrafted Popcorn declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Poppy Handcrafted Popcorn
provider_slug: poppy-handcrafted-popcorn
scheme_count: 5
schemes:
- applies_to: 'POST https://poppyhandcraftedpopcorn.com/api/ucp/mcp (method: tools/list)'
  evidence: tools/list returned HTTP 200 with the full 13-tool schema set and no credential.
  id: anonymous_mcp_discovery
  note: Schema discovery is genuinely open - no key, no token, no signup.
  type: none
  verified: probed
- applies_to: 'POST https://poppyhandcraftedpopcorn.com/api/ucp/mcp (method: tools/call)'
  evidence: tools/call without the field returns HTTP 422 / JSON-RPC -32001 with data.code invalid_profile_url ("Missing profile uri"). tools/call with a URI the server cannot fetch returns HTTP 422 / -32001 with data.code profile_unreachable ("Http error").
  id: ucp_agent_profile
  note: The server resolves the agent profile document over HTTP before executing a tool, so the caller must publish a reachable UCP agent profile. This is a real gate, not a declaration.
  parameter: meta.ucp-agent.profile
  required: true
  type: agent-identity (dereferenced URI)
  verified: probed
- applies_to: 'POST /api/ucp/mcp (method: tools/call) - at least some tools'
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: 'A tools/call naming an unknown tool returned HTTP 403 / JSON-RPC -32000 "AuthenticationRequired" with data "Unauthorized: A valid JWT is required to call <tool>. See https://shopify.dev/docs/agents/get-started/authentication".'
  id: shopify_agent_jwt
  note: Profile resolution is checked BEFORE the JWT check, so our probe could not reach the auth layer for a real tool such as search_catalog - we could not establish which of the 13 tools are callable without a JWT. Recorded as observed on the tools/call path, not asserted for every tool.
  type: http bearer (JWT)
  verified: probed
- applies_to:
  - https://poppyhandcraftedpopcorn.com/products.json
  - https://poppyhandcraftedpopcorn.com/collections/{handle}/products.json
  - https://poppyhandcraftedpopcorn.com/products/{handle}.json
  evidence: HTTP 200 unauthenticated.
  id: anonymous_storefront_json
  type: none
  verified: probed
- applies_to: Customer account operations (order history, saved addresses, payment methods)
  authorization_endpoint: https://shopify.com/authentication/42483876008/oauth/authorize
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_accounts_oidc
  issuer: https://shopify.com/authentication/42483876008
  jwks_uri: https://shopify.com/authentication/42483876008/.well-known/jwks.json
  note: The authorization server is Shopify-operated but the tenant is Poppy's - the issuer path and the shop_id in /.well-known/ucp are the same identifier, 42483876008, and the protected resource is Poppy's own apex domain.
  protected_resource: https://poppyhandcraftedpopcorn.com
  response_types_supported:
  - code
  scopes: scopes/poppy-handcrafted-popcorn-scopes.yml
  token_endpoint: https://shopify.com/authentication/42483876008/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
slug: poppy-handcrafted-popcorn-authentication
source_filename: poppy-handcrafted-popcorn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://poppyhandcraftedpopcorn.com/.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n  (all HTTP 200), plus an anonymous tools/list against /api/ucp/mcp (HTTP 200).\nnote: >-\n  derive-authentication.py produced nothing because it reads OpenAPI securitySchemes and\n  this provider publishes no OpenAPI. This profile is written from the provider's own\n  live OAuth/OIDC discovery documents instead, which is a stronger source than a derived one.\n\nsummary: >-\n  Three layers, established by probe. Schema discovery (tools/list) and the storefront read JSON\n  are fully anonymous. Executing a tool (tools/call) is NOT anonymous: the server dereferences\n  the caller's UCP agent profile URI and, beyond that, answers AuthenticationRequired pointing at\n  Shopify's agent JWT flow. Customer-account operations sit behind Shopify-hosted OAuth 2.0 /\n  OpenID Connect\
  \ with PKCE. Payment on complete_checkout adds a buyer-approval invariant on top\n  of all of it, which is a consent gate rather than a credential.\n\nschemes:\n- id: anonymous_mcp_discovery\n  type: none\n  applies_to: 'POST https://poppyhandcraftedpopcorn.com/api/ucp/mcp (method: tools/list)'\n  verified: probed\n  evidence: tools/list returned HTTP 200 with the full 13-tool schema set and no credential.\n  note: Schema discovery is genuinely open - no key, no token, no signup.\n- id: ucp_agent_profile\n  type: agent-identity (dereferenced URI)\n  applies_to: 'POST https://poppyhandcraftedpopcorn.com/api/ucp/mcp (method: tools/call)'\n  verified: probed\n  parameter: meta.ucp-agent.profile\n  required: true\n  evidence: >-\n    tools/call without the field returns HTTP 422 / JSON-RPC -32001 with data.code\n    invalid_profile_url (\"Missing profile uri\"). tools/call with a URI the server cannot\n    fetch returns HTTP 422 / -32001 with data.code profile_unreachable (\"Http error\").\n\
  \  note: >-\n    The server resolves the agent profile document over HTTP before executing a tool, so the\n    caller must publish a reachable UCP agent profile. This is a real gate, not a declaration.\n- id: shopify_agent_jwt\n  type: http bearer (JWT)\n  applies_to: 'POST /api/ucp/mcp (method: tools/call) - at least some tools'\n  verified: probed\n  evidence: >-\n    A tools/call naming an unknown tool returned HTTP 403 / JSON-RPC -32000\n    \"AuthenticationRequired\" with data \"Unauthorized: A valid JWT is required to call <tool>.\n    See https://shopify.dev/docs/agents/get-started/authentication\".\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  note: >-\n    Profile resolution is checked BEFORE the JWT check, so our probe could not reach the auth\n    layer for a real tool such as search_catalog - we could not establish which of the 13 tools\n    are callable without a JWT. Recorded as observed on the tools/call path, not asserted for\n    every tool.\n\
  - id: anonymous_storefront_json\n  type: none\n  applies_to:\n  - https://poppyhandcraftedpopcorn.com/products.json\n  - https://poppyhandcraftedpopcorn.com/collections/{handle}/products.json\n  - https://poppyhandcraftedpopcorn.com/products/{handle}.json\n  verified: probed\n  evidence: HTTP 200 unauthenticated.\n- id: shopify_customer_accounts_oidc\n  type: openIdConnect\n  applies_to: Customer account operations (order history, saved addresses, payment methods)\n  verified: probed\n  issuer: https://shopify.com/authentication/42483876008\n  authorization_endpoint: https://shopify.com/authentication/42483876008/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/42483876008/oauth/token\n  jwks_uri: https://shopify.com/authentication/42483876008/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported:\n  - S256\n\
  \  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  bearer_methods_supported:\n  - header\n  protected_resource: https://poppyhandcraftedpopcorn.com\n  scopes: scopes/poppy-handcrafted-popcorn-scopes.yml\n  note: >-\n    The authorization server is Shopify-operated but the tenant is Poppy's - the issuer path\n    and the shop_id in /.well-known/ucp are the same identifier, 42483876008, and the\n    protected resource is Poppy's own apex domain.\n\npayment_authorization:\n  mechanism: buyer approval, not a credential\n  source: https://poppyhandcraftedpopcorn.com/llms.txt\n  rule: >-\n    complete_checkout must not be called without explicit, contemporaneous buyer consent.\n    Handlers offered are Google Pay, Shopify card and Shop Pay; the agent never handles a PAN.\n  idempotency_key_required: true\n\ngaps:\n- No API keys, no client registration and no developer signup exist - this is not a developer\n  API program, so there is nothing to provision.\n\
  - No /.well-known/security.txt (404), so no machine-readable security contact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppy-handcrafted-popcorn/refs/heads/main/authentication/poppy-handcrafted-popcorn-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Snacks
---
