---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: probed
name: Harry S Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mammoth Brands secures its APIs with oauth2, openIdConnect, and none across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mammoth Brands
provider_slug: harry-s
scheme_count: 4
schemes:
- authorizationUrl: https://shopify.com/authentication/88395284786/oauth/authorize
  brand: Harry's
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/88395284786/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/88395284786
  jwks_uri: https://shopify.com/authentication/88395284786/.well-known/jwks.json
  name: shopify-customer-account-oidc-harrys
  openIdConnectUrl: https://harrys.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/harry-s-harrys-openid-configuration.json
  subject_types_supported:
  - public
  tokenUrl: https://shopify.com/authentication/88395284786/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorizationUrl: https://shopify.com/authentication/55874814054/oauth/authorize
  brand: Flamingo
  issuer: https://shopify.com/authentication/55874814054
  name: shopify-customer-account-oidc-flamingo
  openIdConnectUrl: https://www.shopflamingo.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/harry-s-flamingo-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/55874814054/oauth/token
  type: openIdConnect
- description: The Harry's and Flamingo storefront MCP endpoints (/api/mcp) accept an unauthenticated JSON-RPC POST. tools/list, search_catalog, get_product_details and the policy search tool all answered anonymously on 2026-07-31. Carts are addressed by an opaque cart_id rather than by a session token.
  name: storefront-mcp-anonymous
  surfaces:
  - https://www.harrys.com/api/mcp
  - https://www.shopflamingo.com/api/mcp
  type: none
- description: The UCP-branded MCP endpoint (/api/ucp/mcp on the myshopify origin) rejects calls without an agent profile URI, returning JSON-RPC -32001 UCP discovery failed / invalid_profile_url. Agent identity, not a bearer token, is the gate.
  name: ucp-agent-profile
  surfaces:
  - https://com-harrys-us.myshopify.com/api/ucp/mcp
  - https://shop-flamingo-us.myshopify.com/api/ucp/mcp
  type: agent-profile
slug: harry-s-authentication
source_filename: harry-s-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://harrys.com/.well-known/openid-configuration\nnote: >-\n  No OpenAPI exists for any Mammoth Brands surface, so this profile was NOT derived from a\n  spec. It was probed live: both Shopify-hosted brands serve a real OpenID Connect / RFC 8414\n  discovery document from their own apex domain, and the storefront MCP endpoints were\n  confirmed to require no authentication at all.\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces: 2\nschemes:\n- name: shopify-customer-account-oidc-harrys\n  type: openIdConnect\n  brand: Harry's\n  openIdConnectUrl: https://harrys.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/88395284786\n  authorizationUrl: https://shopify.com/authentication/88395284786/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/88395284786/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/88395284786/logout\n\
  \  jwks_uri: https://shopify.com/authentication/88395284786/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  subject_types_supported: [public]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/harry-s-harrys-openid-configuration.json]\n- name: shopify-customer-account-oidc-flamingo\n  type: openIdConnect\n  brand: Flamingo\n  openIdConnectUrl: https://www.shopflamingo.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/55874814054\n  authorizationUrl: https://shopify.com/authentication/55874814054/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/55874814054/oauth/token\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n\
  \  sources: [well-known/harry-s-flamingo-openid-configuration.json]\n- name: storefront-mcp-anonymous\n  type: none\n  description: >-\n    The Harry's and Flamingo storefront MCP endpoints (/api/mcp) accept an unauthenticated\n    JSON-RPC POST. tools/list, search_catalog, get_product_details and the policy search tool\n    all answered anonymously on 2026-07-31. Carts are addressed by an opaque cart_id rather\n    than by a session token.\n  surfaces: ['https://www.harrys.com/api/mcp', 'https://www.shopflamingo.com/api/mcp']\n- name: ucp-agent-profile\n  type: agent-profile\n  description: >-\n    The UCP-branded MCP endpoint (/api/ucp/mcp on the myshopify origin) rejects calls without\n    an agent profile URI, returning JSON-RPC -32001 UCP discovery failed / invalid_profile_url.\n    Agent identity, not a bearer token, is the gate.\n  surfaces: ['https://com-harrys-us.myshopify.com/api/ucp/mcp', 'https://shop-flamingo-us.myshopify.com/api/ucp/mcp']\nx-evidence:\n  fetched: '2026-07-31'\n\
  \  documents:\n  - {url: 'https://harrys.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://harrys.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://www.shopflamingo.com/.well-known/openid-configuration', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harry-s/refs/heads/main/authentication/harry-s-authentication.yml
summary_line: oauth2/openIdConnect/none · 4 schemes
tags:
- Company
- Consumer Packaged Goods
- Retail
- E-Commerce
- Personal Care
- Agentic Commerce
- Model Context Protocol
- Shopify
---
