---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: probed
name: David Protein Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: David Protein secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: David Protein
provider_slug: david-protein
scheme_count: 4
schemes:
- applies_to:
  - david-protein-customer-account-mcp
  authorization_url: https://account.davidprotein.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_url: https://account.davidprotein.com/authentication/logout
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/63247417511
  jwks_uri: https://account.davidprotein.com/authentication/.well-known/jwks.json
  name: customer-account-oauth
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/david-protein-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  token_url: https://account.davidprotein.com/authentication/oauth/token
  type: oauth2
- claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  name: openid-connect
  openid_connect_url: https://davidprotein.com/.well-known/openid-configuration
  source: well-known/david-protein-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
- applies_to:
  - david-protein-ucp-commerce-mcp
  bearerFormat: JWT
  name: ucp-agent-jwt
  note: 'An anonymous tools/call on the UCP commerce endpoint returns JSON-RPC error -32000 "AuthenticationRequired" with the message "Unauthorized: A valid JWT is required to call <tool>. See https://shopify.dev/docs/agents/get-started/authentication". tools/list itself is anonymous.'
  scheme: bearer
  source: probe of https://davidprotein.com/api/ucp/mcp
  type: http
- applies_to:
  - david-protein-storefront-mcp
  - david-protein-storefront-json
  name: none
  note: The storefront MCP server at /api/mcp answered both tools/list and a search_catalog tools/call anonymously on probe, as did every /products.json and /collections.json read path documented in agents.md.
  type: none
slug: david-protein-authentication
source_filename: david-protein-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://davidprotein.com/.well-known/openid-configuration\ndocs: https://davidprotein.com/agents.md\nnote: >-\n  David publishes no OpenAPI, so this profile is probed from the live discovery documents\n  the store serves and from the authentication errors the MCP endpoints actually returned,\n  not derived from a spec.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  bearer_methods: [header]\n  pkce: [S256]\nschemes:\n- name: customer-account-oauth\n  type: oauth2\n  source: well-known/david-protein-openid-configuration.json\n  issuer: https://shopify.com/authentication/63247417511\n  authorization_url: https://account.davidprotein.com/authentication/oauth/authorize\n  token_url: https://account.davidprotein.com/authentication/oauth/token\n  end_session_url: https://account.davidprotein.com/authentication/logout\n\
  \  jwks_uri: https://account.davidprotein.com/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  applies_to: [david-protein-customer-account-mcp]\n- name: openid-connect\n  type: openIdConnect\n  source: well-known/david-protein-openid-configuration.json\n  openid_connect_url: https://davidprotein.com/.well-known/openid-configuration\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  subject_types: [public]\n- name: ucp-agent-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  source: probe of https://davidprotein.com/api/ucp/mcp\n  applies_to: [david-protein-ucp-commerce-mcp]\n  note: >-\n    An anonymous tools/call on the UCP commerce endpoint returns JSON-RPC error -32000\n    \"AuthenticationRequired\" with the message \"Unauthorized: A valid JWT is required\
  \ to\n    call <tool>. See https://shopify.dev/docs/agents/get-started/authentication\". tools/list\n    itself is anonymous.\n- name: none\n  type: none\n  applies_to: [david-protein-storefront-mcp, david-protein-storefront-json]\n  note: >-\n    The storefront MCP server at /api/mcp answered both tools/list and a search_catalog\n    tools/call anonymously on probe, as did every /products.json and /collections.json\n    read path documented in agents.md.\nprotected_resource:\n  source: well-known/david-protein-oauth-protected-resource.json\n  resource: https://davidprotein.com\n  authorization_servers:\n  - https://account.davidprotein.com\n  - https://shopify.com/authentication/63247417511\n  bearer_methods_supported: [header]\nx-evidence:\n  fetched: '2026-08-11'\n  urls:\n  - {url: https://davidprotein.com/.well-known/openid-configuration, status: 200}\n  - {url: https://davidprotein.com/.well-known/oauth-authorization-server, status: 200}\n  - {url: https://davidprotein.com/.well-known/oauth-protected-resource,\
  \ status: 200}\n  - {url: https://account.davidprotein.com/authentication/.well-known/jwks.json, status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/david-protein/refs/heads/main/authentication/david-protein-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Agents
- MCP
- Universal Commerce Protocol
- Commerce
- E-Commerce
- Shopping
- Catalog
- Checkout
- Nutrition
- Food and Beverage
- Consumer Packaged Goods
- Shopify
---
