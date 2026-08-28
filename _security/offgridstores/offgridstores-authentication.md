---
api_key_in: []
auth_types: []
description: Off Grid Stores publishes no OpenAPI, so this profile is built from the OAuth/OIDC discovery documents its own host serves and from live authenticated-vs-anonymous probes of each surface. The authorization server is Shopify's customer-account issuer bound to this shop, with all user-facing endpoints on account.offgridstores.com.
kind: authentication
layout: security
method: probed
name: Offgridstores Authentication
name_suffix: Authentication
oauth_flows: []
overview: Off Grid Stores - All Things Off-Grid Solar declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Off Grid Stores - All Things Off-Grid Solar
provider_slug: offgridstores
scheme_count: 0
schemes: []
slug: offgridstores-authentication
source_filename: offgridstores-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://offgridstores.com/.well-known/oauth-authorization-server,\n  https://offgridstores.com/.well-known/oauth-protected-resource, live MCP and GraphQL probes\n  2026-08-26\ndocs: https://shopify.dev/docs/agents/get-started/authentication\ndescription: >-\n  Off Grid Stores publishes no OpenAPI, so this profile is built from the OAuth/OIDC discovery\n  documents its own host serves and from live authenticated-vs-anonymous probes of each surface. The\n  authorization server is Shopify's customer-account issuer bound to this shop, with all user-facing\n  endpoints on account.offgridstores.com.\nsurfaces:\n- surface: Storefront GraphQL API\n  endpoint: https://offgridstores.com/api/2025-10/graphql.json\n  scheme: none\n  type: public\n  probed: '2026-08-26'\n  note: >-\n    Answered a full introspection query (422 types) and a shop/paymentSettings query with no\n    Authorization header and no X-Shopify-Storefront-Access-Token.\
  \ Customer-scoped fields still\n    require a customer access token minted by customerAccessTokenCreate.\n- surface: Storefront MCP server\n  endpoint: https://offgridstores.com/api/mcp\n  scheme: none\n  type: public\n  probed: '2026-08-26'\n  note: tools/list and tools/call both succeeded anonymously.\n- surface: UCP Commerce MCP server\n  endpoint: https://offgridstores.com/api/ucp/mcp\n  scheme: none\n  type: agent-profile\n  probed: '2026-08-26'\n  note: >-\n    tools/list is anonymous. tools/call returns HTTP 422 with JSON-RPC error -32001 \"UCP discovery\n    failed\" / invalid_profile_url until a resolvable agent profile URI is supplied in\n    meta.ucp-agent.profile, which every tool's inputSchema marks required. The agent profile is an\n    identity document, not a bearer credential; Shopify's agent-authentication docs cover the JWT\n    that accompanies it.\n- surface: Storefront JSON endpoints\n  endpoint: https://offgridstores.com/products.json\n  scheme: none\n  type: public\n\
  \  probed: '2026-08-26'\n- surface: Customer Account\n  endpoint: https://account.offgridstores.com/authentication/oauth/authorize\n  scheme: oauth2\n  type: authorization_code\n  probed: '2026-08-26'\nsecuritySchemes:\n- name: customerAccountOAuth\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  code_challenge_methods_supported: [S256]\n  issuer: https://shopify.com/authentication/55184621620\n  authorization_endpoint: https://account.offgridstores.com/authentication/oauth/authorize\n  token_endpoint: https://account.offgridstores.com/authentication/oauth/token\n  end_session_endpoint: https://account.offgridstores.com/authentication/logout\n  jwks_uri: https://account.offgridstores.com/authentication/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  scopes:\
  \ [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  document: well-known/offgridstores-oauth-authorization-server.json\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://offgridstores.com/.well-known/openid-configuration\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types_supported: [public]\n  document: well-known/offgridstores-openid-configuration.json\n- name: ucpAgentProfile\n  type: apiKey\n  in: body\n  field: meta.ucp-agent.profile\n  applies_to: https://offgridstores.com/api/ucp/mcp\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  note: A URI resolving to the calling agent's UCP profile; required on every tools/call.\n- name: customerAccessToken\n  type: apiKey\n  in: header\n  header: X-Shopify-Customer-Access-Token\n  applies_to: Storefront GraphQL customer-scoped fields and mutations\nprotected_resource:\n  resource: https://offgridstores.com\n  authorization_servers:\
  \ [https://account.offgridstores.com, 'https://shopify.com/authentication/55184621620']\n  bearer_methods_supported: [header]\n  rfc: RFC 9728\n  document: well-known/offgridstores-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offgridstores/refs/heads/main/authentication/offgridstores-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- off-grid solar
- renewable energy
- backup power
- solar generators
- LiFePO4 batteries
- inverters
- homesteading
- Agentic Commerce
- MCP
- GraphQL
- UCP
---
