---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Abcoffee Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Abcoffee secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Abcoffee
provider_slug: abcoffee
scheme_count: 3
schemes:
- authorizationUrl: https://shopify.com/authentication/54968025206/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/54968025206/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/54968025206
  jwks_uri: https://shopify.com/authentication/54968025206/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://abcoffee.in/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  sources:
  - well-known/abcoffee-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/54968025206/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to:
  - mcp:get_order
  bearerFormat: JWT
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: 'A tools/call for get_order without a token returns JSON-RPC error -32000 "AuthenticationRequired" with HTTP 403 and the message "Unauthorized: A valid JWT is required to call get_order. See https://shopify.dev/docs/agents/get-started/authentication".'
  name: shopify-agent-jwt
  scheme: bearer
  sources:
  - 'probe: POST https://abcoffee.in/api/ucp/mcp tools/call get_order'
  type: http
- description: Every MCP tool requires meta["ucp-agent"].profile - a URI pointing at the calling agent's UCP profile. It is an agent-identity requirement rather than an authorization credential; omitting it returns JSON-RPC -32001 "UCP discovery failed" / invalid_profile_url with HTTP 422.
  name: ucp-agent-profile
  sources:
  - mcp/abcoffee-mcp-tools.json
  type: other
slug: abcoffee-authentication
source_filename: abcoffee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://abcoffee.in/.well-known/openid-configuration,\n  https://abcoffee.in/.well-known/oauth-authorization-server,\n  https://abcoffee.in/.well-known/oauth-protected-resource,\n  live MCP probes of https://abcoffee.in/api/ucp/mcp\nnote: >-\n  Derived from discovery documents fetched from abcoffee's own host, not from an OpenAPI - abcoffee\n  publishes no OpenAPI. The authorization server is Shopify's Customer Account platform\n  (issuer https://shopify.com/authentication/54968025206), which is the identity provider Shopify\n  hosts for this store; the RFC 9728 protected-resource document served at abcoffee.in names\n  abcoffee.in as the resource and that issuer as its authorization server.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surface: true\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://abcoffee.in/.well-known/openid-configuration\n\
  \  issuer: https://shopify.com/authentication/54968025206\n  authorizationUrl: https://shopify.com/authentication/54968025206/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/54968025206/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/54968025206/logout\n  jwks_uri: https://shopify.com/authentication/54968025206/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  sources: [well-known/abcoffee-openid-configuration.json]\n- name: shopify-agent-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to:\n  - 'mcp:get_order'\n  evidence: >-\n    A tools/call for get_order without a token returns JSON-RPC error -32000 \"AuthenticationRequired\"\n    with HTTP 403 and the message \"Unauthorized: A valid JWT is required to call\
  \ get_order. See\n    https://shopify.dev/docs/agents/get-started/authentication\".\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  sources: ['probe: POST https://abcoffee.in/api/ucp/mcp tools/call get_order']\n- name: ucp-agent-profile\n  type: other\n  description: >-\n    Every MCP tool requires meta[\"ucp-agent\"].profile - a URI pointing at the calling agent's UCP\n    profile. It is an agent-identity requirement rather than an authorization credential; omitting it\n    returns JSON-RPC -32001 \"UCP discovery failed\" / invalid_profile_url with HTTP 422.\n  sources: [mcp/abcoffee-mcp-tools.json]\nanonymous_access:\n  description: >-\n    MCP initialize and tools/list are callable with no credential at all (HTTP 200). The read-only\n    storefront surface documented in llms.txt (/products/{handle}.json,\n    /collections/{handle}/products.json, /search) is also unauthenticated.\n  evidence:\n  - {url: 'https://abcoffee.in/api/ucp/mcp', method: 'tools/list', status:\
  \ 200}\n  - {url: 'https://abcoffee.in/api/ucp/mcp', method: 'initialize', status: 200}\n  - {url: 'https://abcoffee.in/products.json', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcoffee/refs/heads/main/authentication/abcoffee-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Company
- Coffee
- Food and Beverage
- Retail
- Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
- India
- Subscriptions
---
