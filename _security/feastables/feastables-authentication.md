---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
- ucp-agent-profile
description: 'Feastables publishes no OpenAPI, so this profile is derived from live probes of the store''s own /.well-known/ discovery documents plus its /agents.md agent instructions. Three distinct authentication postures coexist: the Storefront MCP server is anonymous, the UCP Shopping MCP server is gated on a UCP agent profile identity, and customer-account access runs on Shopify-hosted OAuth 2.0 / OpenID Connect.'
kind: authentication
layout: security
method: probed
name: Feastables Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Feastables secures its APIs with none, oauth2, openIdConnect, and ucp-agent-profile across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Feastables
provider_slug: feastables
scheme_count: 5
schemes:
- applies_to: https://feastables.com/api/mcp
  description: The Storefront MCP server accepts JSON-RPC initialize and tools/list with no credential. Probed 2026-08-01, HTTP 200.
  name: anonymous-storefront-mcp
  sources:
  - mcp/feastables-mcp.yml
  type: none
- applies_to: https://feastables.com
  description: The read-only storefront JSON endpoints documented in /agents.md (/products.json, /products/{handle}.json, /collections/{handle}/products.json, /search) require no credential.
  name: anonymous-storefront-json
  sources:
  - skills/feastables-agents.md
  type: none
- applies_to: https://feastables.com/api/ucp/mcp
  description: Every UCP Shopping MCP call requires a meta.ucp-agent.profile URI - a URL to the calling platform's UCP profile document, mapped to the HTTP UCP-Agent header. Calls without it are rejected with JSON-RPC -32001 / invalid_profile_url at HTTP 422. This is caller identity, not a bearer credential.
  header: UCP-Agent
  name: ucp-agent-profile
  required_field: meta.ucp-agent.profile
  sources:
  - mcp/feastables-mcp.yml
  spec: https://ucp.dev/2026-04-08/specification/overview/
  type: agent-identity
- authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize
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
  description: Customer-account identity is delegated to Shopify's hosted authentication service for this shop id. PKCE (S256) is supported; the only response type is the authorization code.
  endSessionUrl: https://shopify.com/authentication/55160602784/logout
  grant_types_supported:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/55160602784
  jwksUrl: https://shopify.com/authentication/55160602784/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://feastables.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/feastables-openid-configuration.json
  subject_types_supported:
  - public
  tokenUrl: https://shopify.com/authentication/55160602784/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/55160602784
  bearer_methods_supported:
  - header
  description: RFC 8414 authorization-server metadata mirrors the OIDC document. RFC 9728 protected-resource metadata names https://feastables.com as the protected resource, with bearer tokens carried in the Authorization header.
  flows:
  - authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize
    flow: authorizationCode
    scopes_count: 4
    tokenUrl: https://shopify.com/authentication/55160602784/oauth/token
  name: shopify-customer-account-oauth2
  resource: https://feastables.com
  sources:
  - well-known/feastables-oauth-authorization-server.json
  - well-known/feastables-oauth-protected-resource.json
  type: oauth2
slug: feastables-authentication
source_filename: feastables-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: well-known/feastables-well-known.yml\ndocs: https://feastables.com/agents.md\ndescription: >-\n  Feastables publishes no OpenAPI, so this profile is derived from live probes of\n  the store's own /.well-known/ discovery documents plus its /agents.md agent\n  instructions. Three distinct authentication postures coexist: the Storefront MCP\n  server is anonymous, the UCP Shopping MCP server is gated on a UCP agent profile\n  identity, and customer-account access runs on Shopify-hosted OAuth 2.0 / OpenID\n  Connect.\nsummary:\n  types: [none, oauth2, openIdConnect, ucp-agent-profile]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces: 2\nschemes:\n  - name: anonymous-storefront-mcp\n    type: none\n    description: >-\n      The Storefront MCP server accepts JSON-RPC initialize and tools/list with no\n      credential. Probed 2026-08-01, HTTP 200.\n    applies_to: https://feastables.com/api/mcp\n    sources:\
  \ [mcp/feastables-mcp.yml]\n  - name: anonymous-storefront-json\n    type: none\n    description: >-\n      The read-only storefront JSON endpoints documented in /agents.md\n      (/products.json, /products/{handle}.json, /collections/{handle}/products.json,\n      /search) require no credential.\n    applies_to: https://feastables.com\n    sources: [skills/feastables-agents.md]\n  - name: ucp-agent-profile\n    type: agent-identity\n    description: >-\n      Every UCP Shopping MCP call requires a meta.ucp-agent.profile URI - a URL to\n      the calling platform's UCP profile document, mapped to the HTTP UCP-Agent\n      header. Calls without it are rejected with JSON-RPC -32001 / invalid_profile_url\n      at HTTP 422. This is caller identity, not a bearer credential.\n    applies_to: https://feastables.com/api/ucp/mcp\n    header: UCP-Agent\n    required_field: meta.ucp-agent.profile\n    spec: https://ucp.dev/2026-04-08/specification/overview/\n    sources: [mcp/feastables-mcp.yml]\n\
  \  - name: shopify-customer-account-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://feastables.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/55160602784\n    authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/55160602784/oauth/token\n    jwksUrl: https://shopify.com/authentication/55160602784/.well-known/jwks.json\n    endSessionUrl: https://shopify.com/authentication/55160602784/logout\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n \
  \   description: >-\n      Customer-account identity is delegated to Shopify's hosted authentication\n      service for this shop id. PKCE (S256) is supported; the only response type is\n      the authorization code.\n    sources: [well-known/feastables-openid-configuration.json]\n  - name: shopify-customer-account-oauth2\n    type: oauth2\n    description: >-\n      RFC 8414 authorization-server metadata mirrors the OIDC document. RFC 9728\n      protected-resource metadata names https://feastables.com as the protected\n      resource, with bearer tokens carried in the Authorization header.\n    resource: https://feastables.com\n    authorization_servers: [https://shopify.com/authentication/55160602784]\n    bearer_methods_supported: [header]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/55160602784/oauth/token\n        scopes_count: 4\n    sources:\n\
  \      - well-known/feastables-oauth-authorization-server.json\n      - well-known/feastables-oauth-protected-resource.json\nnotes:\n  - >-\n    No security.txt and no API key programme were found; Feastables does not run a\n    developer key-issuance surface of its own.\n  - >-\n    /account and /account/login return HTTP 406 to non-browser clients, so the\n    customer sign-up/login page could not be verified and is not recorded.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n    - https://feastables.com/.well-known/openid-configuration\n    - https://feastables.com/.well-known/oauth-authorization-server\n    - https://feastables.com/.well-known/oauth-protected-resource\n    - https://feastables.com/api/mcp\n    - https://feastables.com/api/ucp/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feastables/refs/heads/main/authentication/feastables-authentication.yml
summary_line: none/oauth2/openIdConnect/ucp-agent-profile · 5 schemes
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Chocolate
- E-Commerce
- Retail
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
---
