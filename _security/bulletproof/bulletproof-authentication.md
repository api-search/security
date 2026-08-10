---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
- bearer
description: ''
kind: authentication
layout: security
method: probed
name: Bulletproof Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BulletProof secures its APIs with none, oauth2, openIdConnect, and bearer across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BulletProof
provider_slug: bulletproof
scheme_count: 6
schemes:
- applies_to: https://shop.bulletproof.com/api/{version}/graphql.json
  evidence:
    http_status: 200
    url: https://shop.bulletproof.com/api/2026-01/graphql.json
  name: storefront-graphql-anonymous
  observed: Introspection and data queries (shop, products, cart) returned HTTP 200 with no X-Shopify-Storefront-Access-Token header and no cookie. access-control-allow-origin is "*". Cost is reported per request via shopify-complexity-score headers and the extensions.cost field.
  type: none
- applies_to: https://shop.bulletproof.com/products.json, /collections.json, /products/{handle}.json
  evidence:
    http_status: 200
    url: https://shop.bulletproof.com/products.json
  name: storefront-json-anonymous
  observed: HTTP 200 unauthenticated; documented as the read-only agent surface in agents.md.
  type: none
- applies_to: https://www.bulletproof.com/wp-json/
  evidence:
    http_status: 200
    url: https://www.bulletproof.com/wp-json/
  name: wordpress-rest-anonymous
  observed: The route index reports an empty "authentication" array — no authentication scheme is advertised for the public read routes across 16 namespaces / 384 routes.
  type: none
- applies_to: https://shop.bulletproof.com/api/ucp/mcp
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence:
    http_status: 403
    url: https://shop.bulletproof.com/api/ucp/mcp
  name: ucp-agent-profile
  observed: tools/list and initialize answer anonymously. Every tools/call requires a resolvable meta["ucp-agent"].profile URI; without one the server returns JSON-RPC -32001 "UCP discovery failed". Order and checkout tools additionally return JSON-RPC -32000 "AuthenticationRequired — a valid JWT is required".
  scheme: jwt
  type: bearer
- applies_to: https://account.bulletproof.com
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.bulletproof.com/authentication/logout
  evidence:
    http_status: 200
    url: https://shop.bulletproof.com/.well-known/openid-configuration
  flows:
  - authorizationUrl: https://account.bulletproof.com/authentication/oauth/authorize
    flow: authorizationCode
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://account.bulletproof.com/authentication/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/434700319
  jwks_uri: https://account.bulletproof.com/authentication/.well-known/jwks.json
  name: customer-accounts-oidc
  openIdConnectUrl: https://shop.bulletproof.com/.well-known/openid-configuration
  response_types_supported:
  - code
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- applies_to: https://account.bulletproof.com
  evidence:
    http_status: 200
    url: https://shop.bulletproof.com/.well-known/oauth-authorization-server
  metadata: RFC 8414 authorization server metadata, identical payload to the OIDC document
  name: customer-accounts-oauth2
  protected_resource_metadata: RFC 9728 at /.well-known/oauth-protected-resource on shop., account. and myshopify hosts
  type: oauth2
slug: bulletproof-authentication
source_filename: bulletproof-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource:\n- https://shop.bulletproof.com/.well-known/openid-configuration\n- https://shop.bulletproof.com/.well-known/oauth-authorization-server\n- https://shop.bulletproof.com/.well-known/oauth-protected-resource\n- live probes of the Storefront GraphQL and UCP MCP endpoints\nnote: >-\n  Bulletproof publishes no OpenAPI, so nothing here is derived from securitySchemes.\n  Every scheme below was observed live on 2026-08-08 — three of the four surfaces\n  answered anonymously, which is itself the finding.\nsummary:\n  types: [none, oauth2, openIdConnect, bearer]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces: 3\n  gated_surfaces: 2\nschemes:\n- name: storefront-graphql-anonymous\n  type: none\n  applies_to: https://shop.bulletproof.com/api/{version}/graphql.json\n  observed: >-\n    Introspection and data queries (shop, products, cart) returned HTTP 200 with no\n    X-Shopify-Storefront-Access-Token header\
  \ and no cookie. access-control-allow-origin\n    is \"*\". Cost is reported per request via shopify-complexity-score headers and the\n    extensions.cost field.\n  evidence:\n    http_status: 200\n    url: https://shop.bulletproof.com/api/2026-01/graphql.json\n- name: storefront-json-anonymous\n  type: none\n  applies_to: https://shop.bulletproof.com/products.json, /collections.json, /products/{handle}.json\n  observed: HTTP 200 unauthenticated; documented as the read-only agent surface in agents.md.\n  evidence:\n    http_status: 200\n    url: https://shop.bulletproof.com/products.json\n- name: wordpress-rest-anonymous\n  type: none\n  applies_to: https://www.bulletproof.com/wp-json/\n  observed: >-\n    The route index reports an empty \"authentication\" array — no authentication scheme\n    is advertised for the public read routes across 16 namespaces / 384 routes.\n  evidence:\n    http_status: 200\n    url: https://www.bulletproof.com/wp-json/\n- name: ucp-agent-profile\n  type:\
  \ bearer\n  scheme: jwt\n  applies_to: https://shop.bulletproof.com/api/ucp/mcp\n  observed: >-\n    tools/list and initialize answer anonymously. Every tools/call requires a resolvable\n    meta[\"ucp-agent\"].profile URI; without one the server returns JSON-RPC -32001\n    \"UCP discovery failed\". Order and checkout tools additionally return JSON-RPC -32000\n    \"AuthenticationRequired — a valid JWT is required\".\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  evidence:\n    http_status: 403\n    url: https://shop.bulletproof.com/api/ucp/mcp\n- name: customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://shop.bulletproof.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/434700319\n  applies_to: https://account.bulletproof.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.bulletproof.com/authentication/oauth/authorize\n    tokenUrl: https://account.bulletproof.com/authentication/oauth/token\n\
  \    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  jwks_uri: https://account.bulletproof.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.bulletproof.com/authentication/logout\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  response_types_supported: [code]\n  subject_types_supported: [public]\n  evidence:\n    http_status: 200\n    url: https://shop.bulletproof.com/.well-known/openid-configuration\n- name: customer-accounts-oauth2\n  type: oauth2\n  applies_to: https://account.bulletproof.com\n  metadata: RFC 8414 authorization server metadata, identical payload to the OIDC document\n  protected_resource_metadata: RFC 9728 at /.well-known/oauth-protected-resource on shop., account. and myshopify\
  \ hosts\n  evidence:\n    http_status: 200\n    url: https://shop.bulletproof.com/.well-known/oauth-authorization-server\ngaps:\n- The provider publishes no first-party authentication documentation; the only auth guidance\n  reachable from a Bulletproof host is the shopify.dev link embedded in an MCP error message.\n- No /.well-known/security.txt on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulletproof/refs/heads/main/authentication/bulletproof-authentication.yml
summary_line: none/oauth2/openIdConnect/bearer · 6 schemes
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Health and Wellness
- Supplements
- Ecommerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
---
