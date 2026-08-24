---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Glowbar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glowbar declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Glowbar
provider_slug: glowbar
scheme_count: 3
schemes:
- applies_to: MCP tools/list on https://glowbar.com/api/ucp/mcp
  description: Tool discovery is fully anonymous. A POST of {"jsonrpc":"2.0","id":1,"method":"tools/list"} with no credentials returned HTTP 200 and 13 tools with complete input schemas on 2026-08-22.
  evidence:
    http_status: 200
    url: https://glowbar.com/api/ucp/mcp
    verified: '2026-08-22'
  id: anonymous_mcp_discovery
  type: none
- applies_to: every MCP tools/call invocation
  description: 'Every tool''s inputSchema requires a `meta.ucp-agent.profile` property — a URI identifying the calling agent, which the store dereferences. This is an agent identity requirement rather than a bearer credential: there is no API key to obtain and no registration form. A tools/call without it fails closed.'
  evidence:
    http_status: 422
    url: https://glowbar.com/api/ucp/mcp
    verified: '2026-08-22'
  failure:
    error_code: invalid_profile_url
    http_status: 422
    jsonrpc_error_code: -32001
    message: 'UCP discovery failed — Unable to fetch agent profile: Missing profile uri'
  id: ucp_agent_profile
  location: JSON-RPC params.arguments.meta.ucp-agent.profile
  required: true
  type: agent-profile-uri
- applies_to: buyer-scoped data (customer account, saved addresses, order history)
  authorization_endpoint: https://shopify.com/authentication/44884033689/oauth/authorize
  bearer_methods_supported:
  - header
  description: Shopify Customer Accounts, provisioned for Glowbar's shop id 44884033689. Authorization code flow with PKCE (S256), refresh tokens, and a JWT-bearer grant. Bearer tokens are presented in the Authorization header per the RFC 9728 protected-resource document.
  end_session_endpoint: https://shopify.com/authentication/44884033689/logout
  evidence:
    http_status: 200
    url: https://glowbar.com/.well-known/openid-configuration
    verified: '2026-08-22'
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_accounts
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/44884033689
  jwks_uri: https://shopify.com/authentication/44884033689/.well-known/jwks.json
  pkce:
  - S256
  protected_resource: https://glowbar.com
  provenance_note: The authorization server is Shopify's, on shopify.com, not on a Glowbar host. It is recorded here because the discovery documents are served from glowbar.com and the issuer is scoped to Glowbar's shop. This is a platform-provided identity surface, not one Glowbar operates.
  response_types:
  - code
  scopes: scopes/glowbar-scopes.yml
  sub_type: openIdConnect
  token_endpoint: https://shopify.com/authentication/44884033689/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: glowbar-authentication
source_filename: glowbar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://glowbar.com/.well-known/openid-configuration + https://glowbar.com/.well-known/oauth-protected-resource + live POST to https://glowbar.com/api/ucp/mcp\ndocs: https://glowbar.com/agents.md\nnote: >-\n  Glowbar publishes no OpenAPI, so this profile is built from machine-readable discovery\n  documents actually fetched from glowbar.com plus observed behaviour of the live MCP\n  endpoint. There are three distinct authentication postures on this provider and they are\n  not interchangeable.\nschemes:\n- id: anonymous_mcp_discovery\n  type: none\n  applies_to: MCP tools/list on https://glowbar.com/api/ucp/mcp\n  description: >-\n    Tool discovery is fully anonymous. A POST of {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}\n    with no credentials returned HTTP 200 and 13 tools with complete input schemas on\n    2026-08-22.\n  evidence:\n    url: https://glowbar.com/api/ucp/mcp\n    http_status: 200\n    verified:\
  \ '2026-08-22'\n- id: ucp_agent_profile\n  type: agent-profile-uri\n  applies_to: every MCP tools/call invocation\n  description: >-\n    Every tool's inputSchema requires a `meta.ucp-agent.profile` property — a URI identifying\n    the calling agent, which the store dereferences. This is an agent identity requirement\n    rather than a bearer credential: there is no API key to obtain and no registration form.\n    A tools/call without it fails closed.\n  required: true\n  location: JSON-RPC params.arguments.meta.ucp-agent.profile\n  failure:\n    http_status: 422\n    jsonrpc_error_code: -32001\n    error_code: invalid_profile_url\n    message: 'UCP discovery failed — Unable to fetch agent profile: Missing profile uri'\n  evidence:\n    url: https://glowbar.com/api/ucp/mcp\n    http_status: 422\n    verified: '2026-08-22'\n- id: shopify_customer_accounts\n  type: oauth2\n  sub_type: openIdConnect\n  applies_to: buyer-scoped data (customer account, saved addresses, order history)\n  description:\
  \ >-\n    Shopify Customer Accounts, provisioned for Glowbar's shop id 44884033689. Authorization\n    code flow with PKCE (S256), refresh tokens, and a JWT-bearer grant. Bearer tokens are\n    presented in the Authorization header per the RFC 9728 protected-resource document.\n  issuer: https://shopify.com/authentication/44884033689\n  authorization_endpoint: https://shopify.com/authentication/44884033689/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/44884033689/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/44884033689/logout\n  jwks_uri: https://shopify.com/authentication/44884033689/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  bearer_methods_supported: [header]\n  protected_resource: https://glowbar.com\n\
  \  scopes: scopes/glowbar-scopes.yml\n  provenance_note: >-\n    The authorization server is Shopify's, on shopify.com, not on a Glowbar host. It is\n    recorded here because the discovery documents are served from glowbar.com and the issuer\n    is scoped to Glowbar's shop. This is a platform-provided identity surface, not one\n    Glowbar operates.\n  evidence:\n    url: https://glowbar.com/.well-known/openid-configuration\n    http_status: 200\n    verified: '2026-08-22'\nnot_present:\n  api_keys: No API key programme, developer registration, or key-issuance surface is published on any Glowbar host.\n  mutual_tls: Not advertised.\n  http_basic: Not advertised.\n  developer_program: >-\n    Glowbar publishes no developer portal, no API reference and no self-serve credentials.\n    The only machine surface is the platform-provided UCP/MCP endpoint above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glowbar/refs/heads/main/authentication/glowbar-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Skincare
- Beauty
- Retail
- Commerce
- Ecommerce
- Consumer Services
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Memberships
---
