---
api_key_in: []
auth_types: []
description: 'MAKEUP BY MARIO has no developer program and issues no API keys, so there is no developer-facing auth page to read. What exists instead is a two-tier model that was established by probe: everything public about the store — catalog, cart, checkout scaffolding, policies — is reachable with NO credential at all, and only customer-account data sits behind OpenID Connect. That first tier is the unusual part. Three independent machine-readable surfaces on this host answered anonymously with HTTP 200 on 2026-08-25.'
kind: authentication
layout: security
method: probed
name: Makeup By Mario Authentication
name_suffix: Authentication
oauth_flows: []
overview: Makeup by Mario declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Makeup by Mario
provider_slug: makeup-by-mario
scheme_count: 5
schemes:
- applies_to:
  - https://www.makeupbymario.com/api/2026-04/graphql.json
  - https://www.makeupbymario.com/api/mcp
  - https://www.makeupbymario.com/api/ucp/mcp
  - https://www.makeupbymario.com/products.json
  evidence: Full GraphQL introspection, MCP initialize, and MCP tools/list on both servers all returned 200 with no Authorization header and no X-Shopify-Storefront-Access-Token. This is a Shopify configuration choice, not an oversight in our probe — the same probe returns 401/403 on stores that require a storefront token.
  id: anonymous-storefront
  note: Anonymous does not mean unbounded. The GraphQL API is query-cost throttled and the MCP endpoints are rate-limited per IP; see rate-limits/.
  type: none
  verified: '2026-08-25'
- applies_to:
  - https://www.makeupbymario.com/api/ucp/mcp
  evidence: 'Required on all thirteen UCP tools'' inputSchema. resources/list and prompts/list without it return JSON-RPC error -32001 "UCP discovery failed", data.code invalid_profile_url, content "Unable to fetch agent profile: Missing profile uri".'
  format: URI
  id: ucp-agent-profile
  location: JSON-RPC params
  note: This is identity, not authorization — the agent declares who it is by publishing a resolvable profile document, and the server fetches it. There is no secret, no issuance step and no revocation surface. It is the only credential-shaped requirement on the whole agent surface.
  parameter: meta["ucp-agent"].profile
  required: true
  type: agent-profile
  verified: '2026-08-25'
- applies_to:
  - https://www.makeupbymario.com/api/ucp/mcp
  id: complete-checkout-idempotency
  note: Not an auth scheme, recorded here because it is the second required member of the same meta object. See conventions/ for the full treatment.
  parameter: meta["idempotency-key"]
  required: true
  scope: complete_checkout only
  type: idempotency-key
  verified: '2026-08-25'
- applies_to: customer account data (orders, addresses, saved payment methods)
  authorization_endpoint: https://shopify.com/authentication/27548221505/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/27548221505/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/27548221505
  jwks_uri: https://shopify.com/authentication/27548221505/.well-known/jwks.json
  note: 'The issuer is per-merchant — it carries this store''s Shopify shop id 27548221505 — so the discovery document is specific to MAKEUP BY MARIO even though the authorization server is operated by Shopify. Note the fourth scope, customer-account-mcp-api:full: an authenticated customer-account MCP surface is declared here that no anonymous probe can reach.'
  oauth_authorization_server: https://www.makeupbymario.com/.well-known/oauth-authorization-server
  openid_configuration: https://www.makeupbymario.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  token_endpoint: https://shopify.com/authentication/27548221505/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: '2026-08-25'
- applies_to:
  - https://www.makeupbymario.com/api/2026-04/graphql.json
  header: X-Shopify-Customer-Access-Token
  id: storefront-customer-access-token
  note: Minted by the customerAccessTokenCreate mutation. This is the older Storefront-API customer path, coexisting with the OIDC customer-account path above.
  required_for: QueryRoot.customer and the 13 customer* mutations
  type: apiKey
  verified: derived from graphql/makeup-by-mario-storefront.graphql
slug: makeup-by-mario-authentication
source_filename: makeup-by-mario-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://www.makeupbymario.com/.well-known/openid-configuration +\n  https://www.makeupbymario.com/.well-known/oauth-authorization-server + live anonymous\n  probes of the GraphQL, Storefront MCP and UCP MCP endpoints\ndescription: >-\n  MAKEUP BY MARIO has no developer program and issues no API keys, so there is no\n  developer-facing auth page to read. What exists instead is a two-tier model that was\n  established by probe: everything public about the store — catalog, cart, checkout\n  scaffolding, policies — is reachable with NO credential at all, and only customer-account\n  data sits behind OpenID Connect. That first tier is the unusual part. Three independent\n  machine-readable surfaces on this host answered anonymously with HTTP 200 on 2026-08-25.\nschemes:\n- id: anonymous-storefront\n  type: none\n  applies_to:\n  - https://www.makeupbymario.com/api/2026-04/graphql.json\n  - https://www.makeupbymario.com/api/mcp\n\
  \  - https://www.makeupbymario.com/api/ucp/mcp\n  - https://www.makeupbymario.com/products.json\n  verified: '2026-08-25'\n  evidence: >-\n    Full GraphQL introspection, MCP initialize, and MCP tools/list on both servers all\n    returned 200 with no Authorization header and no\n    X-Shopify-Storefront-Access-Token. This is a Shopify configuration choice, not an\n    oversight in our probe — the same probe returns 401/403 on stores that require a\n    storefront token.\n  note: >-\n    Anonymous does not mean unbounded. The GraphQL API is query-cost throttled and the MCP\n    endpoints are rate-limited per IP; see rate-limits/.\n- id: ucp-agent-profile\n  type: agent-profile\n  applies_to: [https://www.makeupbymario.com/api/ucp/mcp]\n  parameter: meta[\"ucp-agent\"].profile\n  location: JSON-RPC params\n  required: true\n  format: URI\n  verified: '2026-08-25'\n  evidence: >-\n    Required on all thirteen UCP tools' inputSchema. resources/list and prompts/list without\n    it return\
  \ JSON-RPC error -32001 \"UCP discovery failed\", data.code invalid_profile_url,\n    content \"Unable to fetch agent profile: Missing profile uri\".\n  note: >-\n    This is identity, not authorization — the agent declares who it is by publishing a\n    resolvable profile document, and the server fetches it. There is no secret, no\n    issuance step and no revocation surface. It is the only credential-shaped requirement\n    on the whole agent surface.\n- id: complete-checkout-idempotency\n  type: idempotency-key\n  applies_to: [https://www.makeupbymario.com/api/ucp/mcp]\n  parameter: meta[\"idempotency-key\"]\n  required: true\n  scope: complete_checkout only\n  verified: '2026-08-25'\n  note: >-\n    Not an auth scheme, recorded here because it is the second required member of the same\n    meta object. See conventions/ for the full treatment.\n- id: customer-account-oidc\n  type: openIdConnect\n  openid_configuration: https://www.makeupbymario.com/.well-known/openid-configuration\n\
  \  oauth_authorization_server: https://www.makeupbymario.com/.well-known/oauth-authorization-server\n  issuer: https://shopify.com/authentication/27548221505\n  authorization_endpoint: https://shopify.com/authentication/27548221505/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/27548221505/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/27548221505/logout\n  jwks_uri: https://shopify.com/authentication/27548221505/.well-known/jwks.json\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  applies_to: customer account data (orders, addresses, saved payment methods)\n\
  \  verified: '2026-08-25'\n  note: >-\n    The issuer is per-merchant — it carries this store's Shopify shop id 27548221505 — so\n    the discovery document is specific to MAKEUP BY MARIO even though the authorization\n    server is operated by Shopify. Note the fourth scope,\n    customer-account-mcp-api:full: an authenticated customer-account MCP surface is\n    declared here that no anonymous probe can reach.\n- id: storefront-customer-access-token\n  type: apiKey\n  header: X-Shopify-Customer-Access-Token\n  applies_to: [https://www.makeupbymario.com/api/2026-04/graphql.json]\n  required_for: QueryRoot.customer and the 13 customer* mutations\n  verified: derived from graphql/makeup-by-mario-storefront.graphql\n  note: >-\n    Minted by the customerAccessTokenCreate mutation. This is the older Storefront-API\n    customer path, coexisting with the OIDC customer-account path above.\ntiers:\n- tier: public\n  credential: none\n  reaches: catalog, collections, editorial content, store\
  \ policies, cart, checkout scaffolding, localisation\n- tier: agent\n  credential: a resolvable UCP agent profile URI\n  reaches: all thirteen UCP commerce tools including complete_checkout\n- tier: customer\n  credential: OIDC authorization code + PKCE, or a Storefront customer access token\n  reaches: that customer's orders, addresses and saved payment methods\nabsent:\n- No developer portal, no API key issuance, no OAuth client registration for third parties.\n- No mutual TLS, no HTTP signatures, no bearer-token scheme of the brand's own.\n- No /.well-known/security.txt and no /.well-known/oauth-protected-resource.\ndocs: https://www.makeupbymario.com/agents.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeup-by-mario/refs/heads/main/authentication/makeup-by-mario-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Beauty
- Cosmetics
- Consumer Packaged Goods
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
