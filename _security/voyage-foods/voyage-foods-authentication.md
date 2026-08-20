---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- http
- none
- agent-profile
description: ''
kind: authentication
layout: security
method: searched
name: Voyage Foods Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Voyage Foods secures its APIs with openIdConnect, oauth2, http, none, and agent-profile across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Voyage Foods
provider_slug: voyage-foods
scheme_count: 6
schemes:
- applies_to: Customer account sign-in and the Shopify Customer Account API / Customer Account MCP API
  authorization_endpoint: https://shopify.com/authentication/59465728192/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/59465728192/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/59465728192
  jwks_uri: https://shopify.com/authentication/59465728192/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://voyagefoods.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/voyage-foods-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/59465728192/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- metadata_url: https://voyagefoods.com/.well-known/oauth-authorization-server
  name: ShopifyOAuthAuthorizationServer
  note: The RFC 8414 authorization-server metadata document is byte-identical to the OIDC discovery document above; the same issuer serves both.
  sources:
  - well-known/voyage-foods-oauth-authorization-server.json
  spec: RFC 8414
  type: oauth2
- applies_to: https://voyagefoods.com/api/2026-04/graphql.json
  customer_token_mutations:
  - customerAccessTokenCreate
  - customerAccessTokenCreateWithMultipass
  - customerAccessTokenRenew
  - customerAccessTokenDelete
  name: StorefrontGraphQLAnonymous
  observed: Anonymous POST returns HTTP 200 for both a trivial query and a full introspection query — no X-Shopify-Storefront-Access-Token was supplied. Public storefront reads (products, collections, search, cart) are unauthenticated; the `customer` query requires a customer access token obtained via the customerAccessTokenCreate mutation or the OIDC flow above.
  sources:
  - graphql/voyage-foods-storefront.graphql
  type: none
- applies_to: https://voyagefoods.com/api/ucp/mcp
  name: UCPAgentProfile
  observed: 'tools/list is answered anonymously (HTTP 200, 13 tools). Tool INVOCATION is not anonymous, and is gated twice. First gate: every tool''s inputSchema requires meta["ucp-agent"].profile, a URI identifying the calling agent, which the server DEREFERENCES — omitting it returns JSON-RPC -32001 / invalid_profile_url, and supplying an unreachable URI returns -32001 / profile_unreachable. This is agent identity, not a bearer credential.'
  required_field: meta.ucp-agent.profile
  sources:
  - mcp/voyage-foods-ucp-tools-list.json
  spec: https://ucp.dev/2026-04-08/specification/overview/
  type: agent-profile
- applies_to: https://voyagefoods.com/api/ucp/mcp
  bearerFormat: JWT
  docs: https://shopify.dev/docs/agents/get-started/authentication
  name: ShopifyAgentJWT
  observed: 'Second gate on tool invocation. A tools/call reached past the discovery check returns JSON-RPC -32000 "AuthenticationRequired" with the detail "Unauthorized: A valid JWT is required to call <tool>. See https://shopify.dev/docs/agents/get-started/authentication for instructions on generating a token and authenticating your requests." Token issuance is a Shopify platform flow, not a Voyage Foods one; the storefront publishes no developer signup of its own.'
  scheme: bearer
  sources:
  - errors/voyage-foods-problem-types.yml
  type: http
- applies_to: https://voyagefoods.com/products.json
  name: StorefrontJSONAnonymous
  observed: Read-only product and collection JSON endpoints return HTTP 200 with no credential.
  sources:
  - llms/voyage-foods-agents.md
  type: none
slug: voyage-foods-authentication
source_filename: voyage-foods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://voyagefoods.com/.well-known/openid-configuration\ndocs: https://voyagefoods.com/agents.md\nnote: >-\n  Voyage Foods publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  assembled from three surfaces probed live on 2026-08-05: the OIDC / RFC 8414 discovery documents\n  served at voyagefoods.com/.well-known/, the anonymous access posture of the Storefront GraphQL\n  endpoint and the UCP/MCP endpoint, and the agent-access rules the store publishes in agents.md,\n  llms.txt and robots.txt.\nsummary:\n  types: [openIdConnect, oauth2, http, none, agent-profile]\n  oauth2_flows: [authorizationCode, refreshToken, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  api_key_in: []\n  http_schemes: [bearer]\n  anonymous_surfaces: 3\n  pkce_required_methods: [S256]\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://voyagefoods.com/.well-known/openid-configuration\n\
  \  issuer: https://shopify.com/authentication/59465728192\n  authorization_endpoint: https://shopify.com/authentication/59465728192/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/59465728192/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/59465728192/logout\n  jwks_uri: https://shopify.com/authentication/59465728192/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  applies_to: Customer account sign-in and the Shopify Customer Account API / Customer Account\
  \ MCP API\n  sources: [well-known/voyage-foods-openid-configuration.json]\n- name: ShopifyOAuthAuthorizationServer\n  type: oauth2\n  spec: RFC 8414\n  metadata_url: https://voyagefoods.com/.well-known/oauth-authorization-server\n  note: >-\n    The RFC 8414 authorization-server metadata document is byte-identical to the OIDC discovery\n    document above; the same issuer serves both.\n  sources: [well-known/voyage-foods-oauth-authorization-server.json]\n- name: StorefrontGraphQLAnonymous\n  type: none\n  applies_to: https://voyagefoods.com/api/2026-04/graphql.json\n  observed: >-\n    Anonymous POST returns HTTP 200 for both a trivial query and a full introspection query — no\n    X-Shopify-Storefront-Access-Token was supplied. Public storefront reads (products, collections,\n    search, cart) are unauthenticated; the `customer` query requires a customer access token obtained\n    via the customerAccessTokenCreate mutation or the OIDC flow above.\n  customer_token_mutations: [customerAccessTokenCreate,\
  \ customerAccessTokenCreateWithMultipass, customerAccessTokenRenew, customerAccessTokenDelete]\n  sources: [graphql/voyage-foods-storefront.graphql]\n- name: UCPAgentProfile\n  type: agent-profile\n  applies_to: https://voyagefoods.com/api/ucp/mcp\n  observed: >-\n    tools/list is answered anonymously (HTTP 200, 13 tools). Tool INVOCATION is not anonymous, and is\n    gated twice. First gate: every tool's inputSchema requires meta[\"ucp-agent\"].profile, a URI\n    identifying the calling agent, which the server DEREFERENCES — omitting it returns JSON-RPC\n    -32001 / invalid_profile_url, and supplying an unreachable URI returns -32001 /\n    profile_unreachable. This is agent identity, not a bearer credential.\n  required_field: meta.ucp-agent.profile\n  spec: https://ucp.dev/2026-04-08/specification/overview/\n  sources: [mcp/voyage-foods-ucp-tools-list.json]\n- name: ShopifyAgentJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: https://voyagefoods.com/api/ucp/mcp\n\
  \  observed: >-\n    Second gate on tool invocation. A tools/call reached past the discovery check returns JSON-RPC\n    -32000 \"AuthenticationRequired\" with the detail \"Unauthorized: A valid JWT is required to call\n    <tool>. See https://shopify.dev/docs/agents/get-started/authentication for instructions on\n    generating a token and authenticating your requests.\" Token issuance is a Shopify platform flow,\n    not a Voyage Foods one; the storefront publishes no developer signup of its own.\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  sources: [errors/voyage-foods-problem-types.yml]\n- name: StorefrontJSONAnonymous\n  type: none\n  applies_to: https://voyagefoods.com/products.json\n  observed: Read-only product and collection JSON endpoints return HTTP 200 with no credential.\n  sources: [llms/voyage-foods-agents.md]\npayment_authorization:\n  human_approval_required: true\n  statement: >-\n    \"Checkout requires human approval. Agents must not complete\
  \ payment without explicit buyer\n    consent.\" — published verbatim in llms.txt and agents.md, and restated in robots.txt.\n  handlers:\n  - {id: gpay, handler: com.google.pay}\n  - {id: shopify.card, handler: dev.shopify.card}\n  - {id: shop_pay, handler: dev.shopify.shop_pay}\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://voyagefoods.com/.well-known/openid-configuration', http_status: 200, content_type: application/json}\n  - {url: 'https://voyagefoods.com/.well-known/oauth-authorization-server', http_status: 200, content_type: application/json}\n  - {url: 'https://voyagefoods.com/api/2026-04/graphql.json', http_status: 200, note: anonymous introspection succeeded}\n  - {url: 'https://voyagefoods.com/api/ucp/mcp', http_status: 200, note: anonymous tools/list succeeded; initialize without an agent profile returned JSON-RPC -32001}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyage-foods/refs/heads/main/authentication/voyage-foods-authentication.yml
summary_line: openIdConnect/oauth2/http/none/agent-profile · 6 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- Food Technology
---
