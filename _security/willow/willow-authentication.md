---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Willow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Willow declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Willow
provider_slug: willow
scheme_count: 4
schemes:
- applies_to:
  - MCP initialize
  - MCP tools/list
  - GET /.well-known/ucp.json
  - GET /agents.md
  - GET /llms.txt
  - GET /products.json
  - GET /collections/{handle}/products.json
  evidence: POST {"jsonrpc":"2.0","id":1,"method":"tools/list"} to https://onewillow.com/api/ucp/mcp returned HTTP 200 with 13 tools and no credential of any kind on 2026-09-04.
  id: anonymous-discovery
  type: none
- applies_to: every tools/call invocation
  description: 'Each tool''s inputSchema requires meta["ucp-agent"].profile — a URI the server dereferences to resolve the calling agent''s UCP profile. It is an identity/provenance requirement rather than a secret: no key is issued by Willow, but a call without a resolvable profile is rejected.'
  evidence: Observed 2026-09-04 by calling tools/call search_catalog with, and then without, a well-formed profile URI.
  failure_modes:
  - code: -32001
    data_code: invalid_profile_url
    message: 'UCP discovery failed: Unable to fetch agent profile: Missing profile uri'
  - code: -32001
    data_code: profile_malformed
    message: 'UCP discovery failed: Unable to fetch agent profile: Invalid content type'
  format: uri
  id: ucp-agent-profile
  in: json-rpc params
  location: params.arguments.meta["ucp-agent"].profile
  required: true
  type: agent-identity
- applies_to:
  - get_order
  - order-scoped and buyer-scoped operations
  bearer_format: JWT
  description: Order retrieval requires a signed agent JWT. Willow does not document the issuance flow itself; the server's own error body points at Shopify's agent authentication documentation.
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: 'tools/call get_order returned JSON-RPC error -32000 "AuthenticationRequired — Unauthorized: A valid JWT is required to call get_order." on 2026-09-04.'
  id: agent-jwt
  scheme: bearer
  type: http
- description: Buyer-facing OAuth 2.0 + OpenID Connect for Willow's customer accounts, issued by Shopify on Willow's shop id 15958015 and served on Willow's own account.onewillow.com host. Note customer-account-mcp-api:full — the customer account surface itself is MCP-addressable.
  end_session_endpoint: https://account.onewillow.com/authentication/logout
  evidence: RFC 8414 / OIDC discovery documents fetched 2026-09-04 (HTTP 200, byte-identical to each other).
  flows:
    authorization_code:
      authorization_url: https://account.onewillow.com/authentication/oauth/authorize
      pkce: S256
      token_url: https://account.onewillow.com/authentication/oauth/token
    jwt_bearer: urn:ietf:params:oauth:grant-type:jwt-bearer
    refresh_token: true
  id: shopify-customer-accounts-oauth
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/15958015
  jwks_uri: https://account.onewillow.com/authentication/.well-known/jwks.json
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: willow-authentication
source_filename: willow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://onewillow.com/.well-known/openid-configuration,\n  https://onewillow.com/.well-known/oauth-authorization-server,\n  https://onewillow.com/.well-known/oauth-protected-resource,\n  https://onewillow.com/api/ucp/mcp (live JSON-RPC probes),\n  https://onewillow.com/agents.md\ndocs: https://onewillow.com/agents.md\nsummary: >-\n  Willow publishes no API key programme and no developer console. The only callable surface is the\n  UCP commerce MCP endpoint on its storefront, which layers three distinct auth models: anonymous\n  discovery, an agent-profile identity requirement for tool calls, and OAuth 2.0 / OIDC (Shopify\n  Customer Accounts) for buyer- and order-scoped access. There is no OpenAPI document, so this\n  profile is built from live probes and the provider's own agent instructions rather than from\n  declared securitySchemes.\nschemes:\n  - id: anonymous-discovery\n    type: none\n    applies_to:\n      - MCP\
  \ initialize\n      - MCP tools/list\n      - GET /.well-known/ucp.json\n      - GET /agents.md\n      - GET /llms.txt\n      - GET /products.json\n      - GET /collections/{handle}/products.json\n    evidence: >-\n      POST {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"} to https://onewillow.com/api/ucp/mcp\n      returned HTTP 200 with 13 tools and no credential of any kind on 2026-09-04.\n  - id: ucp-agent-profile\n    type: agent-identity\n    in: json-rpc params\n    location: params.arguments.meta[\"ucp-agent\"].profile\n    required: true\n    format: uri\n    applies_to: every tools/call invocation\n    description: >-\n      Each tool's inputSchema requires meta[\"ucp-agent\"].profile — a URI the server dereferences to\n      resolve the calling agent's UCP profile. It is an identity/provenance requirement rather than a\n      secret: no key is issued by Willow, but a call without a resolvable profile is rejected.\n    failure_modes:\n      - code: -32001\n        data_code:\
  \ invalid_profile_url\n        message: 'UCP discovery failed: Unable to fetch agent profile: Missing profile uri'\n      - code: -32001\n        data_code: profile_malformed\n        message: 'UCP discovery failed: Unable to fetch agent profile: Invalid content type'\n    evidence: >-\n      Observed 2026-09-04 by calling tools/call search_catalog with, and then without, a well-formed\n      profile URI.\n  - id: agent-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to:\n      - get_order\n      - order-scoped and buyer-scoped operations\n    description: >-\n      Order retrieval requires a signed agent JWT. Willow does not document the issuance flow itself;\n      the server's own error body points at Shopify's agent authentication documentation.\n    docs: https://shopify.dev/docs/agents/get-started/authentication\n    evidence: >-\n      tools/call get_order returned JSON-RPC error -32000 \"AuthenticationRequired — Unauthorized: A\n      valid JWT is required\
  \ to call get_order.\" on 2026-09-04.\n  - id: shopify-customer-accounts-oauth\n    type: oauth2\n    flows:\n      authorization_code:\n        authorization_url: https://account.onewillow.com/authentication/oauth/authorize\n        token_url: https://account.onewillow.com/authentication/oauth/token\n        pkce: S256\n      refresh_token: true\n      jwt_bearer: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    issuer: https://shopify.com/authentication/15958015\n    jwks_uri: https://account.onewillow.com/authentication/.well-known/jwks.json\n    end_session_endpoint: https://account.onewillow.com/authentication/logout\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg:\n      - RS256\n    scopes:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    description: >-\n      Buyer-facing OAuth 2.0 + OpenID Connect for Willow's customer accounts, issued by Shopify\
  \ on\n      Willow's shop id 15958015 and served on Willow's own account.onewillow.com host. Note\n      customer-account-mcp-api:full — the customer account surface itself is MCP-addressable.\n    evidence: >-\n      RFC 8414 / OIDC discovery documents fetched 2026-09-04 (HTTP 200, byte-identical to each other).\nprotected_resources:\n  - resource: https://onewillow.com\n    authorization_servers:\n      - https://account.onewillow.com\n      - https://shopify.com/authentication/15958015\n    bearer_methods_supported:\n      - header\n    rfc: RFC 9728\n    source: https://onewillow.com/.well-known/oauth-protected-resource\napi_keys:\n  issued: false\n  note: Willow publishes no API key, client credential, or developer registration surface of its own.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willow/refs/heads/main/authentication/willow-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Consumer Health
- Breast Pumps
- Maternal Health
- Medical Devices
- Ecommerce
- Agentic Commerce
- MCP
- UCP
- agent-native
- Shopify
---
