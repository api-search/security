---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Slingshot Biosciences Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Slingshot Biosciences secures its APIs with none, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Slingshot Biosciences
provider_slug: slingshot-biosciences
scheme_count: 5
schemes:
- applies_to: https://slingshot-bio.myshopify.com/api/2026-07/graphql.json
  description: 'The Shopify Storefront GraphQL endpoint answers unauthenticated POSTs for shop, product, collection, blog and cart operations, and permits full schema introspection. Verified 2026-08-05: an anonymous query for shop.name and the first three products returned HTTP 200 with real data.'
  evidence:
    http_status: 200
    probe: POST {shop{name} products(first:3){edges{node{id title handle}}}}
  name: anonymous-storefront
  type: none
- applies_to: https://9l0m1rv5.api.sanity.io/v2025-08-29/data/query/production
  description: The Sanity Content Lake production dataset is public-read. An anonymous GROQ query over HTTPS GET returned HTTP 200 with document results.
  evidence:
    http_status: 200
    probe: GET ?query=*[_type=="sanity.imageAsset"][0...1]{_id}
  name: anonymous-content-lake
  type: none
- applies_to: https://slingshot-bio.myshopify.com/api/mcp
  description: MCP tools/list is answered without a token, returning five tools with full inputSchemas.
  evidence:
    http_status: 200
    probe: POST {"jsonrpc":"2.0","id":1,"method":"tools/list"}
  name: anonymous-mcp-discovery
  type: none
- applies_to: https://slingshot-bio.myshopify.com/api/mcp
  bearer_methods_supported:
  - header
  description: Customer-scoped MCP and Customer Account API operations are protected by the OAuth 2.0 authorization server the store advertises via RFC 9728 /.well-known/oauth-protected-resource.
  flows:
  - authorizationUrl: https://shopify.com/authentication/60285812930/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://shopify.com/authentication/60285812930/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/slingshot-biosciences-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
- applies_to: https://shopify.com/authentication/60285812930
  description: 'The same authorization server publishes OpenID Connect discovery metadata: RS256 id_tokens, a JWKS URI, an end_session_endpoint and the openid/email claims set.'
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/60285812930
  jwks_uri: https://shopify.com/authentication/60285812930/.well-known/jwks.json
  name: shopify-customer-account-oidc
  source: well-known/slingshot-biosciences-openid-configuration.json
  type: openIdConnect
slug: slingshot-biosciences-authentication
source_filename: slingshot-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: >-\n  https://slingshot-bio.myshopify.com/.well-known/oauth-authorization-server +\n  live anonymous requests to the storefront GraphQL, Sanity GROQ and MCP endpoints\nnote: >-\n  Slingshot Bio publishes no OpenAPI, so this profile was probed against the live\n  surfaces rather than derived from securitySchemes. All three declared endpoints\n  answer anonymously for read operations; only customer-scoped operations require\n  a token.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  anonymous_read: true\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\nschemes:\n- name: anonymous-storefront\n  type: none\n  applies_to: https://slingshot-bio.myshopify.com/api/2026-07/graphql.json\n  description: >-\n    The Shopify Storefront GraphQL endpoint answers unauthenticated POSTs for\n    shop, product, collection, blog and cart operations, and permits full schema\n    introspection. Verified 2026-08-05: an anonymous query for\
  \ shop.name and the\n    first three products returned HTTP 200 with real data.\n  evidence:\n    http_status: 200\n    probe: 'POST {shop{name} products(first:3){edges{node{id title handle}}}}'\n- name: anonymous-content-lake\n  type: none\n  applies_to: https://9l0m1rv5.api.sanity.io/v2025-08-29/data/query/production\n  description: >-\n    The Sanity Content Lake production dataset is public-read. An anonymous GROQ\n    query over HTTPS GET returned HTTP 200 with document results.\n  evidence:\n    http_status: 200\n    probe: 'GET ?query=*[_type==\"sanity.imageAsset\"][0...1]{_id}'\n- name: anonymous-mcp-discovery\n  type: none\n  applies_to: https://slingshot-bio.myshopify.com/api/mcp\n  description: >-\n    MCP tools/list is answered without a token, returning five tools with full\n    inputSchemas.\n  evidence:\n    http_status: 200\n    probe: 'POST {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  applies_to:\
  \ https://slingshot-bio.myshopify.com/api/mcp\n  description: >-\n    Customer-scoped MCP and Customer Account API operations are protected by the\n    OAuth 2.0 authorization server the store advertises via RFC 9728\n    /.well-known/oauth-protected-resource.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/60285812930/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/60285812930/oauth/token\n    pkce: [S256]\n  bearer_methods_supported: [header]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  source: well-known/slingshot-biosciences-oauth-protected-resource.json\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  applies_to: https://shopify.com/authentication/60285812930\n  description: >-\n    The same authorization server publishes OpenID Connect discovery metadata:\n    RS256 id_tokens, a JWKS URI, an end_session_endpoint and the openid/email\n    claims set.\n  issuer: https://shopify.com/authentication/60285812930\n\
  \  jwks_uri: https://shopify.com/authentication/60285812930/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  source: well-known/slingshot-biosciences-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://slingshot-bio.myshopify.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://slingshot-bio.myshopify.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://slingshot-bio.myshopify.com/api/2026-07/graphql.json\n    http_status: 200\n  - url: https://9l0m1rv5.api.sanity.io/v2025-08-29/data/query/production\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slingshot-biosciences/refs/heads/main/authentication/slingshot-biosciences-authentication.yml
summary_line: none/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Flow Cytometry
- Laboratory
- Synthetic Biology
- Diagnostics
- Cell Therapy
- E-Commerce
- GraphQL
- MCP
---
