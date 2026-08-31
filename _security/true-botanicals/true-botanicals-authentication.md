---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: True Botanicals Authentication
name_suffix: Authentication
oauth_flows: []
overview: True Botanicals declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: True Botanicals
provider_slug: true-botanicals
scheme_count: 3
schemes:
- description: 'Discovery is anonymous but invocation is not. tools/list answered HTTP 200 with no Authorization header on 2026-08-30. tools/call, however, requires a resolvable UCP agent profile in meta.ucp-agent.profile: calling search_catalog with an unresolvable profile URI returned HTTP 422 and JSON-RPC error -32001 "UCP discovery failed" / profile_unreachable, and calling it with no meta at all returns the same -32001 with invalid_profile_url. Order lookup is a further step up: get_order returned HTTP 403 and JSON-RPC -32000 AuthenticationRequired, "A valid JWT is required". So the practical auth model is agent-identity by published profile document for catalog/cart/checkout, and a bearer JWT for order data.'
  id: none-ucp-mcp
  surface: https://truebotanicals.com/api/ucp/mcp
  type: none
  verified: probed
- description: The Shopify Storefront GraphQL endpoint answered full introspection and catalog queries with no X-Shopify-Storefront-Access-Token header. Read access to published catalog data is anonymous on this host.
  id: none-storefront-graphql
  surface: https://truebotanicals.com/api/2026-01/graphql.json
  type: none
  verified: probed
- authorization_endpoint: https://shopify.com/authentication/5451009/oauth/authorize
  code_challenge_methods:
  - S256
  description: OpenID Connect / OAuth 2.0 authorization server for True Botanicals customer accounts, discovered at this merchant's own well-known path and operated by Shopify for shop 5451009. Authorization-code flow with PKCE; refresh tokens and RFC 7523 jwt-bearer grants supported.
  end_session_endpoint: https://shopify.com/authentication/5451009/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/5451009/.well-known/jwks.json
  openIdConnectUrl: https://truebotanicals.com/.well-known/openid-configuration
  response_types:
  - code
  scopes_file: scopes/true-botanicals-scopes.yml
  surface: https://shopify.com/authentication/5451009
  token_endpoint: https://shopify.com/authentication/5451009/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
slug: true-botanicals-authentication
source_filename: true-botanicals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: 'https://truebotanicals.com/.well-known/openid-configuration + /.well-known/oauth-authorization-server\n  (HTTP 200) and live unauthenticated calls to /api/ucp/mcp and /api/2026-01/graphql.json, 2026-08-30'\nsummary: 'True Botanicals issues no API credentials of its own — there is no developer portal, no key signup\n  and no documented auth page. Two of its three machine surfaces are open to anonymous callers; the third,\n  Shopify customer accounts, is a standards-complete OAuth 2.0 / OpenID Connect authorization server operated\n  by Shopify and scoped to this shop.'\nschemes:\n- id: none-ucp-mcp\n  type: none\n  surface: https://truebotanicals.com/api/ucp/mcp\n  description: 'Discovery is anonymous but invocation is not. tools/list answered HTTP 200 with no Authorization\n    header on 2026-08-30. tools/call, however, requires a resolvable UCP agent profile in meta.ucp-agent.profile:\n    calling search_catalog with an unresolvable\
  \ profile URI returned HTTP 422 and JSON-RPC error -32001\n    \"UCP discovery failed\" / profile_unreachable, and calling it with no meta at all returns the same -32001 with\n    invalid_profile_url. Order lookup is a further step up: get_order returned HTTP 403 and JSON-RPC -32000\n    AuthenticationRequired, \"A valid JWT is required\". So the practical auth model is agent-identity by published\n    profile document for catalog/cart/checkout, and a bearer JWT for order data.'\n  verified: probed\n- id: none-storefront-graphql\n  type: none\n  surface: https://truebotanicals.com/api/2026-01/graphql.json\n  description: 'The Shopify Storefront GraphQL endpoint answered full introspection and catalog queries with no\n    X-Shopify-Storefront-Access-Token header. Read access to published catalog data is anonymous on this host.'\n  verified: probed\n- id: shopify-customer-accounts-oidc\n  type: openIdConnect\n  surface: https://shopify.com/authentication/5451009\n  openIdConnectUrl: https://truebotanicals.com/.well-known/openid-configuration\n\
  \  description: 'OpenID Connect / OAuth 2.0 authorization server for True Botanicals customer accounts, discovered\n    at this merchant''s own well-known path and operated by Shopify for shop 5451009. Authorization-code flow with\n    PKCE; refresh tokens and RFC 7523 jwt-bearer grants supported.'\n  authorization_endpoint: https://shopify.com/authentication/5451009/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/5451009/oauth/token\n  jwks_uri: https://shopify.com/authentication/5451009/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/5451009/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes_file: scopes/true-botanicals-scopes.yml\n  verified: probed\nnotes:\n- 'Client registration\
  \ for the customer-accounts authorization server is not open — the discovery document\n  publishes no registration_endpoint, and Shopify issues client ids through the merchant admin. Third parties\n  cannot self-serve credentials against this issuer.'\n- 'No api-key, http-bearer or mutualTLS scheme is documented or observed anywhere on this provider''s surface.'\n- 'An agent that wants to transact here must itself publish a UCP agent profile at a fetchable URI — the\n  authentication burden sits on the caller''s discoverability, not on a credential the merchant issues.'\n- 'The JWT that get_order demands is minted through Shopify''s agent authentication flow, documented at\n  https://shopify.dev/docs/agents/get-started/authentication — a Shopify-platform credential, not a\n  True Botanicals one.'\nx-evidence:\n- url: https://truebotanicals.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-30'\n- url: https://truebotanicals.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n  fetched: '2026-08-30'\n- url: https://truebotanicals.com/api/ucp/mcp\n  http_status: 200\n  note: unauthenticated POST tools/list\n  fetched: '2026-08-30'\n- url: https://truebotanicals.com/api/ucp/mcp\n  http_status: 422\n  note: 'POST tools/call search_catalog with an unresolvable meta.ucp-agent.profile -> -32001 profile_unreachable'\n  fetched: '2026-08-30'\n- url: https://truebotanicals.com/api/ucp/mcp\n  http_status: 403\n  note: 'POST tools/call get_order without a JWT -> -32000 AuthenticationRequired'\n  fetched: '2026-08-30'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-botanicals/refs/heads/main/authentication/true-botanicals-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Retail
- E-Commerce
- Beauty
- Skincare
- Consumer Goods
- Direct to Consumer
- Agentic Commerce
- Shopify
- MCP
- Universal Commerce Protocol
---
