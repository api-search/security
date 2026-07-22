---
api_key_in: []
auth_types: []
description: Authentication profile for the UNTUCKit storefront's agent and customer surfaces, taken verbatim from the store's live RFC 8414 authorization-server metadata and OIDC discovery documents (saved under well-known/). Customer identity is Shopify Customer Accounts (issuer https://shopify.com/authentication/1291072) fronted at account.untuckit.com.
kind: authentication
layout: security
method: searched
name: Untuckit Authentication
name_suffix: Authentication
oauth_flows: []
overview: UNTUCKit declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: UNTUCKit
provider_slug: untuckit
scheme_count: 3
schemes:
- description: OAuth 2.0 + OIDC for the Shopify Customer Account API and the customer-context MCP API. Authorization-code flow with PKCE (S256), refresh tokens, and JWT-bearer grant; client_secret_basic at the token endpoint; RS256 id_tokens.
  end_session_endpoint: https://account.untuckit.com/authentication/logout
  flows:
    authorizationCode:
      authorizationUrl: https://account.untuckit.com/authentication/oauth/authorize
      scopes:
        customer-account-api:full: Full customer-account API access
        customer-account-mcp-api:full: Customer-context MCP API access
        email: Customer email claims
        openid: OpenID Connect authentication
      tokenUrl: https://account.untuckit.com/authentication/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  jwks_uri: https://account.untuckit.com/authentication/.well-known/jwks.json
  name: customer-account-oauth
  pkce: S256
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
- description: 'The UCP/MCP endpoint (https://www.untuckit.com/api/ucp/mcp) gates requests on the Universal Commerce Protocol agent-profile handshake: a live tools/list probe without a profile URI returns JSON-RPC error -32001 invalid_profile_url. Payment completion additionally requires explicit buyer approval (Shop Pay / Google Pay / card handlers declared in well-known/untuckit-ucp.json).'
  name: ucp-agent-profile
  type: custom
- description: 'Read-only storefront data requires no authentication: product and collection JSON (/products/{handle}.json, /collections/{handle}/products.json), search, and sitemap, as documented in agents.md.'
  name: anonymous-read
  type: none
slug: untuckit-authentication
source_filename: untuckit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://untuckit.com/.well-known/oauth-authorization-server\ndocs: https://www.untuckit.com/agents.md\ndescription: >-\n  Authentication profile for the UNTUCKit storefront's agent and customer\n  surfaces, taken verbatim from the store's live RFC 8414 authorization-server\n  metadata and OIDC discovery documents (saved under well-known/). Customer\n  identity is Shopify Customer Accounts (issuer\n  https://shopify.com/authentication/1291072) fronted at account.untuckit.com.\nschemes:\n  - name: customer-account-oauth\n    type: oauth2\n    description: >-\n      OAuth 2.0 + OIDC for the Shopify Customer Account API and the\n      customer-context MCP API. Authorization-code flow with PKCE (S256),\n      refresh tokens, and JWT-bearer grant; client_secret_basic at the token\n      endpoint; RS256 id_tokens.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://account.untuckit.com/authentication/oauth/authorize\n\
  \        tokenUrl: https://account.untuckit.com/authentication/oauth/token\n        scopes:\n          openid: OpenID Connect authentication\n          email: Customer email claims\n          customer-account-api:full: Full customer-account API access\n          customer-account-mcp-api:full: Customer-context MCP API access\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    pkce: S256\n    token_endpoint_auth_methods:\n      - client_secret_basic\n    jwks_uri: https://account.untuckit.com/authentication/.well-known/jwks.json\n    end_session_endpoint: https://account.untuckit.com/authentication/logout\n  - name: ucp-agent-profile\n    type: custom\n    description: >-\n      The UCP/MCP endpoint (https://www.untuckit.com/api/ucp/mcp) gates\n      requests on the Universal Commerce Protocol agent-profile handshake: a\n      live tools/list probe without a profile URI returns JSON-RPC error\n      -32001 invalid_profile_url.\
  \ Payment completion additionally requires\n      explicit buyer approval (Shop Pay / Google Pay / card handlers declared\n      in well-known/untuckit-ucp.json).\n  - name: anonymous-read\n    type: none\n    description: >-\n      Read-only storefront data requires no authentication: product and\n      collection JSON (/products/{handle}.json,\n      /collections/{handle}/products.json), search, and sitemap, as documented\n      in agents.md.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/untuckit/refs/heads/main/authentication/untuckit-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Apparel
- Retail
- eCommerce
- Shopify
- Agentic Commerce
- MCP
- UCP
---
