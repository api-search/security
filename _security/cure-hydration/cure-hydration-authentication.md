---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Cure Hydration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cure Hydration declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cure Hydration
provider_slug: cure-hydration
scheme_count: 4
schemes:
- applies_to:
  - GET /products.json
  - GET /products/{handle}.json
  - GET /collections.json
  - GET /collections/{handle}/products.json
  - GET /meta.json
  - GET /sitemap.xml
  - POST /api/2026-04/graphql.json (introspection observed 200 with no token)
  - POST /api/ucp/mcp (initialize, tools/list)
  id: anonymous
  note: Verified anonymously on 2026-08-11. Full Storefront GraphQL introspection returned 416 types with no X-Shopify-Storefront-Access-Token header present.
  type: none
- applies_to:
  - POST /api/ucp/mcp (tools/call, resources/list)
  evidence:
    fetched: '2026-08-11'
    http_status: 422
    url: https://www.curehydration.com/api/ucp/mcp
  format: URI
  id: ucp-agent-profile
  location: request body
  note: Not a credential. The caller supplies a URI to its own published agent profile and the server fetches it. Omitting it returns JSON-RPC -32001 / invalid_profile_url; supplying an unreachable URI returns -32001 / profile_unreachable over HTTP 422.
  parameter: meta["ucp-agent"].profile
  secret: false
  type: agentIdentity
- applies_to:
  - Shopify Customer Account API
  - Shopify Customer Account MCP API
  authorization_endpoint: https://shopify.com/authentication/7323713602/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/7323713602/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  human_login: https://www.curehydration.com/account/login
  id: shopify-customer-accounts-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/7323713602
  jwks_uri: https://shopify.com/authentication/7323713602/.well-known/jwks.json
  note: Platform-provided. The discovery document is served from Cure's own apex under /.well-known/, but the issuer and all endpoints are Shopify-hosted and scoped to this store's shop id.
  openIdConnectUrl: https://www.curehydration.com/.well-known/openid-configuration
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
  token_endpoint: https://shopify.com/authentication/7323713602/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to:
  - POST /api/{version}/graphql.json
  id: shopify-storefront-access-token
  location: header
  note: The documented credential for the Storefront API. Not required for the introspection and public catalog reads observed here, and Cure publishes no public storefront token and no way to request one — there is no developer portal, no app registration page, and no API terms.
  parameter: X-Shopify-Storefront-Access-Token
  type: apiKey
slug: cure-hydration-authentication
source_filename: cure-hydration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://www.curehydration.com/.well-known/openid-configuration\nsummary: >-\n  Cure Hydration has no API-key programme and no developer credential of its own. Three\n  distinct access models sit on the domain: fully anonymous read (storefront JSON,\n  GraphQL introspection, MCP tools/list), an agent-identity gate on MCP tool invocation\n  (a resolvable UCP agent profile URI, not a secret), and Shopify Customer Accounts\n  OpenID Connect for shopper login.\n\nschemes:\n  - id: anonymous\n    type: none\n    applies_to:\n      - GET /products.json\n      - GET /products/{handle}.json\n      - GET /collections.json\n      - GET /collections/{handle}/products.json\n      - GET /meta.json\n      - GET /sitemap.xml\n      - POST /api/2026-04/graphql.json (introspection observed 200 with no token)\n      - POST /api/ucp/mcp (initialize, tools/list)\n    note: >-\n      Verified anonymously on 2026-08-11. Full Storefront GraphQL introspection\
  \ returned\n      416 types with no X-Shopify-Storefront-Access-Token header present.\n\n  - id: ucp-agent-profile\n    type: agentIdentity\n    location: request body\n    parameter: meta[\"ucp-agent\"].profile\n    format: URI\n    applies_to:\n      - POST /api/ucp/mcp (tools/call, resources/list)\n    secret: false\n    note: >-\n      Not a credential. The caller supplies a URI to its own published agent profile and the\n      server fetches it. Omitting it returns JSON-RPC -32001 / invalid_profile_url; supplying\n      an unreachable URI returns -32001 / profile_unreachable over HTTP 422.\n    evidence:\n      url: https://www.curehydration.com/api/ucp/mcp\n      http_status: 422\n      fetched: '2026-08-11'\n\n  - id: shopify-customer-accounts-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://www.curehydration.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/7323713602\n    authorization_endpoint: https://shopify.com/authentication/7323713602/oauth/authorize\n\
  \    token_endpoint: https://shopify.com/authentication/7323713602/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/7323713602/logout\n    jwks_uri: https://shopify.com/authentication/7323713602/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic]\n    pkce: [S256]\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes:\n      - openid\n      - email\n      - 'customer-account-api:full'\n      - 'customer-account-mcp-api:full'\n    applies_to:\n      - Shopify Customer Account API\n      - Shopify Customer Account MCP API\n    human_login: https://www.curehydration.com/account/login\n    note: >-\n      Platform-provided. The discovery document is served from Cure's own apex under\n      /.well-known/,\
  \ but the issuer and all endpoints are Shopify-hosted and scoped to this\n      store's shop id.\n\n  - id: shopify-storefront-access-token\n    type: apiKey\n    location: header\n    parameter: X-Shopify-Storefront-Access-Token\n    applies_to:\n      - POST /api/{version}/graphql.json\n    note: >-\n      The documented credential for the Storefront API. Not required for the introspection\n      and public catalog reads observed here, and Cure publishes no public storefront token\n      and no way to request one — there is no developer portal, no app registration page,\n      and no API terms.\n\ngaps:\n  - No developer account, API key issuance flow, or credential documentation of any kind is published by Cure.\n  - >-\n    The only auth documentation an integrator gets is Shopify's platform documentation at\n    shopify.dev, linked from the store's own /agents.md and /llms.txt. Cure publishes no\n    first-party auth page.\n\ndocs:\n  - https://www.curehydration.com/agents.md\n  -\
  \ https://www.curehydration.com/llms.txt\n  - https://shopify.dev/docs/api/customer\n  - https://shopify.dev/docs/api/storefront\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cure-hydration/refs/heads/main/authentication/cure-hydration-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Consumer Packaged Goods
- Beverages
- Health and Wellness
- E-Commerce
- Direct to Consumer
- Retail
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
---
