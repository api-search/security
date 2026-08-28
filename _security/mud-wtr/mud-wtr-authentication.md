---
api_key_in: []
auth_types: []
description: MUD\WTR publishes no OpenAPI, so this profile is built from the OAuth/OIDC discovery documents its own host serves and from live authenticated-vs-anonymous probes of each surface. The authorization server is Shopify's customer-account issuer bound to this shop, with all user-facing endpoints on account.mudwtr.com.
kind: authentication
layout: security
method: probed
name: Mud Wtr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mud\Wtr declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Mud\Wtr
provider_slug: mud-wtr
scheme_count: 0
schemes: []
slug: mud-wtr-authentication
source_filename: mud-wtr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://mudwtr.com/.well-known/oauth-authorization-server,\n  https://mudwtr.com/.well-known/oauth-protected-resource, live MCP and GraphQL probes 2026-08-26\ndocs: https://shopify.dev/docs/agents/get-started/authentication\ndescription: >-\n  MUD\\WTR publishes no OpenAPI, so this profile is built from the OAuth/OIDC discovery documents its\n  own host serves and from live authenticated-vs-anonymous probes of each surface. The authorization\n  server is Shopify's customer-account issuer bound to this shop, with all user-facing endpoints on\n  account.mudwtr.com.\nsurfaces:\n- surface: Storefront GraphQL API\n  endpoint: https://mudwtr.com/api/2025-10/graphql.json\n  scheme: none\n  type: public\n  probed: '2026-08-26'\n  note: >-\n    Answered a full introspection query and a shop query with no Authorization header and no\n    X-Shopify-Storefront-Access-Token. Customer-scoped fields still require a customer access token\n\
  \    minted by customerAccessTokenCreate.\n- surface: Storefront MCP server\n  endpoint: https://mudwtr.com/api/mcp\n  scheme: none\n  type: public\n  probed: '2026-08-26'\n  note: tools/list and tools/call both succeeded anonymously.\n- surface: UCP Commerce MCP server\n  endpoint: https://mudwtr.com/api/ucp/mcp\n  scheme: http\n  bearer_format: JWT\n  type: agent-jwt\n  probed: '2026-08-26'\n  note: >-\n    tools/list is anonymous. tools/call returns JSON-RPC error -32000 \"AuthenticationRequired —\n    Unauthorized: A valid JWT is required\", and separately requires a UCP agent profile URI in\n    meta.ucp-agent.profile (error -32001 invalid_profile_url when omitted).\n- surface: Storefront JSON endpoints\n  endpoint: https://mudwtr.com/products.json\n  scheme: none\n  type: public\n  probed: '2026-08-26'\n- surface: Customer Account\n  endpoint: https://account.mudwtr.com/authentication/oauth/authorize\n  scheme: oauth2\n  type: authorization_code\n  probed: '2026-08-26'\nsecuritySchemes:\n\
  - name: customerAccountOAuth\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  code_challenge_methods_supported: [S256]\n  issuer: https://shopify.com/authentication/13794345014\n  authorization_endpoint: https://account.mudwtr.com/authentication/oauth/authorize\n  token_endpoint: https://account.mudwtr.com/authentication/oauth/token\n  end_session_endpoint: https://account.mudwtr.com/authentication/logout\n  jwks_uri: https://account.mudwtr.com/authentication/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  document: well-known/mud-wtr-oauth-authorization-server.json\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://mudwtr.com/.well-known/openid-configuration\n\
  \  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types_supported: [public]\n  document: well-known/mud-wtr-openid-configuration.json\n- name: agentJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: https://mudwtr.com/api/ucp/mcp\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n- name: customerAccessToken\n  type: apiKey\n  in: header\n  header: X-Shopify-Customer-Access-Token\n  applies_to: Storefront GraphQL customer-scoped fields and mutations\nprotected_resource:\n  resource: https://mudwtr.com\n  authorization_servers: [https://account.mudwtr.com, 'https://shopify.com/authentication/13794345014']\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\n  document: well-known/mud-wtr-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mud-wtr/refs/heads/main/authentication/mud-wtr-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Consumer Goods
- Food and Beverage
- Shopify
- Agentic Commerce
- MCP
- GraphQL
- UCP
---
