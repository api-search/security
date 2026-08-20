---
api_key_in:
- header
auth_types:
- none
- openIdConnect
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Coldsnap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ColdSnap secures its APIs with none, openIdConnect, oauth2, and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ColdSnap
provider_slug: coldsnap
scheme_count: 6
schemes:
- applies_to: https://coldsnap.com/api/mcp
  description: The storefront MCP server accepts unauthenticated JSON-RPC. initialize, tools/list, prompts/list and resources/list all returned 200 with no credential. Cart identity is carried by an opaque cart_id rather than by a bearer token.
  name: anonymous-storefront-mcp
  type: none
  verified: true
- applies_to: https://coldsnap.com/api/2026-07/graphql.json
  description: Full GraphQL introspection and shop/product/collection queries succeeded with no X-Shopify-Storefront-Access-Token header. Shopify's documented header for this API is X-Shopify-Storefront-Access-Token (apiKey, in header); it was not required for the anonymous reads observed here.
  documented_header: X-Shopify-Storefront-Access-Token
  name: anonymous-storefront-graphql
  type: none
  verified: true
- applies_to: https://coldsnap.com/products.json
  description: /products.json, /collections.json, /products/{handle}.json, /collections/{handle}/products.json and /cart.js all returned 200 anonymously.
  name: anonymous-json-ajax
  type: none
  verified: true
- applies_to: customer account APIs and the customer-account MCP surface
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods:
  - S256
  description: Customer identity for the store is issued by Shopify's customer-accounts OpenID Provider, discoverable at the ColdSnap origin. Authorization Code with PKCE (S256), RS256 id_tokens, client_secret_basic token endpoint auth.
  endpoints:
    authorization: https://shopify.com/authentication/97378959650/oauth/authorize
    end_session: https://shopify.com/authentication/97378959650/logout
    jwks: https://shopify.com/authentication/97378959650/.well-known/jwks.json
    token: https://shopify.com/authentication/97378959650/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/97378959650
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://coldsnap.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  type: openIdConnect
  verified: true
- applies_to: https://coldsnap.com
  authorization_servers:
  - https://shopify.com/authentication/97378959650
  bearer_methods_supported:
  - header
  description: RFC 9728 protected-resource metadata declares https://coldsnap.com as a protected resource whose authorization server is the Shopify customer-accounts issuer, with bearer tokens carried in the Authorization header.
  flows:
  - authorizationUrl: https://shopify.com/authentication/97378959650/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/97378959650/oauth/token
  name: oauth2-protected-resource
  resource: https://coldsnap.com
  type: oauth2
  verified: true
- applies_to: https://coldsnap.com/api/ucp/mcp
  description: The UCP agentic-commerce MCP endpoint does not accept anonymous tools/list; it requires the calling agent to present a UCP agent profile URI for discovery. Anonymous calls returned HTTP 422 with jsonrpc error -32001 "UCP discovery failed" and data.code invalid_profile_url.
  gated: true
  in: header
  name: ucp-agent-profile
  type: apiKey
  verified: true
slug: coldsnap-authentication
source_filename: coldsnap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://coldsnap.com/.well-known/openid-configuration\ndocs: https://coldsnap.com/agents.md\nnote: >-\n  Derived from live probes rather than from an OpenAPI securitySchemes block - ColdSnap\n  publishes no OpenAPI. The auth surface was read from RFC 8414 / RFC 9728 / OIDC\n  discovery documents served on coldsnap.com and from the observed behaviour of each\n  API surface.\nsummary:\n  types: [none, openIdConnect, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces: 3\nschemes:\n- name: anonymous-storefront-mcp\n  type: none\n  applies_to: https://coldsnap.com/api/mcp\n  description: >-\n    The storefront MCP server accepts unauthenticated JSON-RPC. initialize, tools/list,\n    prompts/list and resources/list all returned 200 with no credential. Cart identity\n    is carried by an opaque cart_id rather than by a bearer token.\n  verified: true\n- name: anonymous-storefront-graphql\n\
  \  type: none\n  applies_to: https://coldsnap.com/api/2026-07/graphql.json\n  description: >-\n    Full GraphQL introspection and shop/product/collection queries succeeded with no\n    X-Shopify-Storefront-Access-Token header. Shopify's documented header for this API\n    is X-Shopify-Storefront-Access-Token (apiKey, in header); it was not required for\n    the anonymous reads observed here.\n  documented_header: X-Shopify-Storefront-Access-Token\n  verified: true\n- name: anonymous-json-ajax\n  type: none\n  applies_to: https://coldsnap.com/products.json\n  description: >-\n    /products.json, /collections.json, /products/{handle}.json, /collections/{handle}/products.json\n    and /cart.js all returned 200 anonymously.\n  verified: true\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://coldsnap.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/97378959650\n  applies_to: customer account APIs and the customer-account\
  \ MCP surface\n  description: >-\n    Customer identity for the store is issued by Shopify's customer-accounts OpenID\n    Provider, discoverable at the ColdSnap origin. Authorization Code with PKCE (S256),\n    RS256 id_tokens, client_secret_basic token endpoint auth.\n  endpoints:\n    authorization: https://shopify.com/authentication/97378959650/oauth/authorize\n    token: https://shopify.com/authentication/97378959650/oauth/token\n    jwks: https://shopify.com/authentication/97378959650/.well-known/jwks.json\n    end_session: https://shopify.com/authentication/97378959650/logout\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  verified: true\n- name: oauth2-protected-resource\n  type: oauth2\n  applies_to:\
  \ https://coldsnap.com\n  description: >-\n    RFC 9728 protected-resource metadata declares https://coldsnap.com as a protected\n    resource whose authorization server is the Shopify customer-accounts issuer, with\n    bearer tokens carried in the Authorization header.\n  resource: https://coldsnap.com\n  authorization_servers: [https://shopify.com/authentication/97378959650]\n  bearer_methods_supported: [header]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/97378959650/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/97378959650/oauth/token\n  verified: true\n- name: ucp-agent-profile\n  type: apiKey\n  in: header\n  applies_to: https://coldsnap.com/api/ucp/mcp\n  description: >-\n    The UCP agentic-commerce MCP endpoint does not accept anonymous tools/list; it\n    requires the calling agent to present a UCP agent profile URI for discovery.\n    Anonymous calls returned HTTP 422 with jsonrpc error -32001 \"UCP discovery\
  \ failed\"\n    and data.code invalid_profile_url.\n  gated: true\n  verified: true\nobserved_agent_differential:\n  note: >-\n    The customer login entry https://coldsnap.com/customer_authentication/login returns\n    HTTP 406 to non-browser clients (both a default curl UA and a spoofed Chrome UA)\n    while correctly issuing the OIDC authorize redirect in the redirect chain. Login\n    is human-gated; the machine surfaces are not.\nx-evidence:\n  fetched: '2026-08-02'\n  sources:\n  - {url: 'https://coldsnap.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://coldsnap.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://coldsnap.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://coldsnap.com/api/mcp', http_status: 200, method: POST}\n  - {url: 'https://coldsnap.com/api/2026-07/graphql.json', http_status: 200, method: POST}\n  - {url: 'https://coldsnap.com/api/ucp/mcp', http_status: 422, method: POST}\n\
  \  - {url: 'https://coldsnap.com/customer_authentication/login', http_status: 406}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coldsnap/refs/heads/main/authentication/coldsnap-authentication.yml
summary_line: none/openIdConnect/oauth2/apiKey · 6 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Food and Beverage
- Consumer Products
- Hardware
- Appliances
- Food Service
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
