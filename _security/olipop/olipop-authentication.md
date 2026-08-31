---
api_key_in:
- header
auth_types:
- none
- apiKey
- oauth2
- openIdConnect
- agent-profile
description: ''
kind: authentication
layout: security
method: searched
name: Olipop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Olipop secures its APIs with none, apiKey, oauth2, openIdConnect, and agent-profile across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Olipop
provider_slug: olipop
scheme_count: 5
schemes:
- applies_to:
  - /products.json
  - /products/{handle}.json
  - /collections/{handle}/products.json
  - /search?q={query}&type=product
  - /sitemap.xml
  description: Product, collection, search, sitemap and policy JSON/HTML require no credential at all.
  name: publicRead
  source: https://drinkolipop.com/llms.txt
  type: none
- applies_to:
  - https://drinkolipop.com/api/2025-07/graphql.json
  description: Public storefront access token for the Shopify Storefront GraphQL API. Schema introspection at https://drinkolipop.com/api/2025-07/graphql.json answered anonymously during this probe; data reads and all mutations require the token.
  in: header
  name: storefrontAccessToken
  parameter_name: X-Shopify-Storefront-Access-Token
  source: https://shopify.dev/docs/api/storefront
  type: apiKey
- applies_to:
  - https://drinkolipop.com/api/2025-07/graphql.json
  description: Per-customer token minted by the customerAccessTokenCreate mutation and passed as an argument to customer-scoped queries and mutations in the Storefront GraphQL schema.
  in: body
  name: customerAccessToken
  parameter_name: customerAccessToken
  source: graphql/olipop-storefront.graphql
  type: apiKey
- authorization_endpoint: https://shopify.com/authentication/3466100806/oauth/authorize
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
  description: Shopify customer accounts OIDC provider scoped to this shop (shop id 3466100806). Also advertised as an RFC 8414 OAuth 2.0 authorization server at /.well-known/oauth-authorization-server with a byte-identical document.
  end_session_endpoint: https://shopify.com/authentication/3466100806/logout
  flows:
  - code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    token_endpoint_auth_methods:
    - client_secret_basic
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/3466100806
  jwks_uri: https://shopify.com/authentication/3466100806/.well-known/jwks.json
  name: shopifyCustomerAccounts
  openIdConnectUrl: https://drinkolipop.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/olipop-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/3466100806/oauth/token
  type: openIdConnect
- applies_to:
  - https://drinkolipop.com/api/ucp/mcp
  description: The UCP/MCP commerce endpoint does not authenticate with a bearer token; it requires the CALLING PLATFORM to identify itself with a URL to its own UCP profile document, carried as meta["ucp-agent"].profile in the JSON-RPC params or as the UCP-Agent HTTP header. An anonymous call is rejected with JSON-RPC -32001 / invalid_profile_url before any tool is exposed. Payment authorization is separate again and rides the declared payment handlers (Google Pay, Shopify Card, Shop Pay) with a mandatory human buyer-approval step.
  in: header
  name: ucpAgentProfile
  parameter_name: UCP-Agent
  source: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json
  type: agent-profile
slug: olipop-authentication
source_filename: olipop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://drinkolipop.com/.well-known/openid-configuration\ndocs: https://drinkolipop.com/agents.md\nnotes: >-\n  OLIPOP publishes no OpenAPI, so this profile was assembled from live probes rather than derived from\n  securitySchemes. Three distinct auth models coexist on the drinkolipop.com host: an unauthenticated\n  read-only JSON/catalog surface, a token-bearing Storefront GraphQL surface, and an agent-identity model\n  (UCP-Agent profile) in front of the MCP commerce endpoint - with OIDC underneath for customer accounts.\nsummary:\n  types: [none, apiKey, oauth2, openIdConnect, agent-profile]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\nschemes:\n- name: publicRead\n  type: none\n  description: Product, collection, search, sitemap and policy JSON/HTML require no credential at all.\n  applies_to:\n  - /products.json\n  - /products/{handle}.json\n  - /collections/{handle}/products.json\n  -\
  \ /search?q={query}&type=product\n  - /sitemap.xml\n  source: https://drinkolipop.com/llms.txt\n- name: storefrontAccessToken\n  type: apiKey\n  in: header\n  parameter_name: X-Shopify-Storefront-Access-Token\n  description: >-\n    Public storefront access token for the Shopify Storefront GraphQL API. Schema introspection at\n    https://drinkolipop.com/api/2025-07/graphql.json answered anonymously during this probe; data reads and\n    all mutations require the token.\n  applies_to: [https://drinkolipop.com/api/2025-07/graphql.json]\n  source: https://shopify.dev/docs/api/storefront\n- name: customerAccessToken\n  type: apiKey\n  in: body\n  parameter_name: customerAccessToken\n  description: >-\n    Per-customer token minted by the customerAccessTokenCreate mutation and passed as an argument to\n    customer-scoped queries and mutations in the Storefront GraphQL schema.\n  applies_to: [https://drinkolipop.com/api/2025-07/graphql.json]\n  source: graphql/olipop-storefront.graphql\n-\
  \ name: shopifyCustomerAccounts\n  type: openIdConnect\n  openIdConnectUrl: https://drinkolipop.com/.well-known/openid-configuration\n  description: >-\n    Shopify customer accounts OIDC provider scoped to this shop (shop id 3466100806). Also advertised as an\n    RFC 8414 OAuth 2.0 authorization server at /.well-known/oauth-authorization-server with a byte-identical\n    document.\n  issuer: https://shopify.com/authentication/3466100806\n  authorization_endpoint: https://shopify.com/authentication/3466100806/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/3466100806/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/3466100806/logout\n  jwks_uri: https://shopify.com/authentication/3466100806/.well-known/jwks.json\n  flows:\n  - flow: authorizationCode\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [client_secret_basic]\n\
  \  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  source: well-known/olipop-openid-configuration.json\n- name: ucpAgentProfile\n  type: agent-profile\n  in: header\n  parameter_name: UCP-Agent\n  description: >-\n    The UCP/MCP commerce endpoint does not authenticate with a bearer token; it requires the CALLING\n    PLATFORM to identify itself with a URL to its own UCP profile document, carried as\n    meta[\"ucp-agent\"].profile in the JSON-RPC params or as the UCP-Agent HTTP header. An anonymous call is\n    rejected with JSON-RPC -32001 / invalid_profile_url before any tool is exposed. Payment authorization\n    is separate again and rides the declared payment handlers (Google Pay, Shopify Card, Shop Pay) with a\n    mandatory human buyer-approval step.\n  applies_to: [https://drinkolipop.com/api/ucp/mcp]\n  source: https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\n\
  x-evidence:\n  fetched: '2026-07-31'\n  probes:\n  - {url: 'https://drinkolipop.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://drinkolipop.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://drinkolipop.com/api/2025-07/graphql.json', method: POST, http_status: 200, note: anonymous introspection succeeded}\n  - {url: 'https://drinkolipop.com/api/ucp/mcp', method: POST, http_status: 422, note: anonymous tools/list rejected}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olipop/refs/heads/main/authentication/olipop-authentication.yml
summary_line: none/apiKey/oauth2/openIdConnect/agent-profile · 5 schemes
tags:
- beverage
- consumer-packaged-goods
- direct-to-consumer
- E-Commerce
- Retail
- agent-commerce
- universal-commerce-protocol
- MCP
- graphql
- shopify
- prebiotic-soda
- functional-beverage
---
