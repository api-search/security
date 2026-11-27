---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cortex Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cortex Gateway declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cortex Gateway
provider_slug: cortex-gateway-dev
scheme_count: 3
schemes:
- description: The gateway is an OAuth 2.1 resource server. OAUTH_ISSUER points at any authorization server "that issues RS256 JWTs with a JWKS endpoint and supports the scope claim"; clients send a Bearer token whose aud is the gateway's canonical URI (CORTEX_CANONICAL_URI, RFC 8707 audience binding).
  discovery: RFC 9728 protected resource metadata; unauthenticated calls get 401 with "WWW-Authenticate Bearer resource_metadata=..."
  format: RS256 JWT
  header: Authorization
  in: header
  name: OAuth 2.1 bearer (resource server)
  standards:
  - RFC 9728
  - RFC 8414
  - RFC 7591
  - RFC 7636
  - RFC 8707
  - RFC 6750
  - RFC 7662
  type: oauth2
- description: CORTEX_TECHNICAL_TOKEN — static token the gateway uses for backend catalog discovery (catalog methods only).
  name: Technical token
  type: apiKey
- description: Local development only; CORTEX_DEV_BYPASS_TOKEN replaces the Bearer JWT, with scopes from CORTEX_DEV_BYPASS_SCOPES (README Quickstart).
  header: X-Dev-Mode
  in: header
  name: Dev bypass
  type: apiKey
slug: cortex-gateway-dev-authentication
source_filename: cortex-gateway-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cortex-gateway.dev/guides/secure-mcp-with-oauth/\ndocs: https://cortex-gateway.dev/guides/secure-mcp-with-oauth/\nschemes:\n- type: oauth2\n  name: OAuth 2.1 bearer (resource server)\n  in: header\n  header: Authorization\n  format: RS256 JWT\n  description: The gateway is an OAuth 2.1 resource server. OAUTH_ISSUER points at\n    any authorization server \"that issues RS256 JWTs with a JWKS endpoint and supports\n    the scope claim\"; clients send a Bearer token whose aud is the gateway's canonical\n    URI (CORTEX_CANONICAL_URI, RFC 8707 audience binding).\n  discovery: RFC 9728 protected resource metadata; unauthenticated calls get 401 with\n    \"WWW-Authenticate Bearer resource_metadata=...\"\n  standards:\n  - RFC 9728\n  - RFC 8414\n  - RFC 7591\n  - RFC 7636\n  - RFC 8707\n  - RFC 6750\n  - RFC 7662\n- type: apiKey\n  name: Technical token\n  description: CORTEX_TECHNICAL_TOKEN — static token the gateway uses\
  \ for backend\n    catalog discovery (catalog methods only).\n- type: apiKey\n  name: Dev bypass\n  in: header\n  header: X-Dev-Mode\n  description: Local development only; CORTEX_DEV_BYPASS_TOKEN replaces the Bearer\n    JWT, with scopes from CORTEX_DEV_BYPASS_SCOPES (README Quickstart).\nidentity_propagation: The caller's JWT is forwarded to first-party backends; federated\n  native MCP servers get the user's own linked OAuth token from a per-user encrypted\n  vault (proxy adapter).\ndocs_also:\n- https://cortex-gateway.dev/answers/mcp-oauth-issuer-behind-proxy/\n- https://github.com/wellknownmcp/cortex-gateway/blob/main/docs/security.md\n"
source_yaml_url: https://artifacts.apis.io/cortex-gateway-dev/authentication/cortex-gateway-dev-authentication.yml
summary_line: 3 schemes
tags:
- Company
- MCP
- MCP Gateway
- Open Source
- OAuth 2.1
- AI Agents
- Identity
- Authorization
- Self-Hosted
---
