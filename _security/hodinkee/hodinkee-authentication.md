---
api_key_in: []
auth_types: []
description: Hodinkee publishes no API keys, no developer registration and no API auth documentation of its own. The auth profile below is read from the live OAuth / OpenID metadata the commerce host serves, plus direct anonymous probes of the two MCP endpoints on 2026-08-22.
kind: authentication
layout: security
method: probed
name: Hodinkee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hodinkee declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Hodinkee
provider_slug: hodinkee
scheme_count: 3
schemes:
- applies_to:
  - https://shop.hodinkee.com/api/ucp/mcp
  - https://shop.hodinkee.com/api/mcp
  - https://shop.hodinkee.com/products.json
  - https://shop.hodinkee.com/collections/{handle}/products.json
  evidence: POST tools/list returned HTTP 200 with the full tool set on both MCP endpoints with no Authorization header. tools/call search_catalog on /api/mcp returned real HODINKEE product data anonymously.
  id: anonymous
  probed: '2026-08-22'
  type: none
- applies_to:
  - Shopify Customer Account API for shop 1460732
  - Customer-scoped MCP API (customer-account-mcp-api:full)
  authorization_endpoint: https://shopify.com/authentication/1460732/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/1460732/logout
  evidence: well-known/hodinkee-shop-openid-configuration.json
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oauth
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/1460732
  jwks_uri: https://shopify.com/authentication/1460732/.well-known/jwks.json
  pkce: S256
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/1460732/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to:
  - https://shop.hodinkee.com/api/ucp/mcp
  description: Not a credential, but a required identity assertion. Every UCP tool takes a mandatory `meta.ucp-agent.profile` URI. Calling tools/call without one returns HTTP 422 and JSON-RPC error -32001 (data.code "invalid_profile_url", "Unable to fetch agent profile"). The agent identifies itself by publishing a profile document, not by presenting a secret.
  id: ucp-agent-profile
  probed: '2026-08-22'
  type: agent-identity
slug: hodinkee-authentication
source_filename: hodinkee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://shop.hodinkee.com/.well-known/openid-configuration\ndocs: https://shop.hodinkee.com/agents.md\nname: HODINKEE Shop authentication profile\ndescription: >-\n  Hodinkee publishes no API keys, no developer registration and no API auth\n  documentation of its own. The auth profile below is read from the live OAuth /\n  OpenID metadata the commerce host serves, plus direct anonymous probes of the\n  two MCP endpoints on 2026-08-22.\nsummary:\n  anonymous_surface: true\n  api_keys: false\n  developer_registration: false\n  note: >-\n    Catalog search, cart and checkout creation over MCP required no credential\n    at all. Only customer-scoped operations sit behind OAuth.\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - https://shop.hodinkee.com/api/ucp/mcp\n  - https://shop.hodinkee.com/api/mcp\n  - https://shop.hodinkee.com/products.json\n  - https://shop.hodinkee.com/collections/{handle}/products.json\n  evidence:\
  \ >-\n    POST tools/list returned HTTP 200 with the full tool set on both MCP\n    endpoints with no Authorization header. tools/call search_catalog on\n    /api/mcp returned real HODINKEE product data anonymously.\n  probed: '2026-08-22'\n- id: shopify-customer-account-oauth\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://shopify.com/authentication/1460732\n  authorization_endpoint: https://shopify.com/authentication/1460732/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/1460732/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/1460732/logout\n  jwks_uri: https://shopify.com/authentication/1460732/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n\
  \  applies_to:\n  - Shopify Customer Account API for shop 1460732\n  - Customer-scoped MCP API (customer-account-mcp-api:full)\n  evidence: well-known/hodinkee-shop-openid-configuration.json\n- id: ucp-agent-profile\n  type: agent-identity\n  applies_to:\n  - https://shop.hodinkee.com/api/ucp/mcp\n  description: >-\n    Not a credential, but a required identity assertion. Every UCP tool takes a\n    mandatory `meta.ucp-agent.profile` URI. Calling tools/call without one\n    returns HTTP 422 and JSON-RPC error -32001\n    (data.code \"invalid_profile_url\", \"Unable to fetch agent profile\"). The\n    agent identifies itself by publishing a profile document, not by presenting\n    a secret.\n  probed: '2026-08-22'\nprotected_resource:\n  rfc: RFC 9728\n  resource: https://shop.hodinkee.com\n  authorization_servers:\n  - https://shopify.com/authentication/1460732\n  bearer_methods_supported:\n  - header\n  file: well-known/hodinkee-shop-oauth-protected-resource.json\nownership_note: >-\n\
  \  The authorization server is Shopify's, scoped to Hodinkee's shop id (1460732).\n  Hodinkee neither operates nor documents an identity provider of its own.\nchecked: '2026-08-22'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hodinkee/refs/heads/main/authentication/hodinkee-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Watches
- Luxury Goods
- E-Commerce
- Media
- Publishing
- Retail
- Agentic Commerce
- Model Context Protocol
- Shopify
---
