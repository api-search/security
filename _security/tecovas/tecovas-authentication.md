---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tecovas Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tecovas secures its APIs with none, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tecovas
provider_slug: tecovas
scheme_count: 3
schemes:
- applies_to:
  - https://www.tecovas.com/api/productdetail/:slug
  - https://www.tecovas.com/api/collection
  - https://www.tecovas.com/api/collection-products
  - https://www.tecovas.com/api/search-settings
  - https://checkout.tecovas.com/api/2026-01/graphql.json
  evidence: agents.md states "This site exposes read-only product, collection, and search APIs — no authentication required." All four endpoints and GraphQL introspection returned 200 anonymously on 2026-08-05.
  name: none
  type: none
- applies_to:
  - https://checkout.tecovas.com/api/ucp/mcp
  description: Every UCP MCP tool requires a meta.ucp-agent.profile URI identifying the calling agent. tools/list is anonymous, but an initialize call without a profile returns JSON-RPC error -32001 invalid_profile_url (HTTP 422).
  evidence: mcp/tecovas-ucp-tools-list.json
  in: request-body
  name: ucp-agent-profile
  parameter: meta.ucp-agent.profile
  required: true
  type: profile
- authorizationUrl: https://accounts.tecovas.com/authentication/oauth/authorize
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
  end_session_endpoint: https://accounts.tecovas.com/authentication/logout
  flows:
  - flow: authorizationCode
    pkce:
    - S256
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/9910824
  jwks_uri: https://accounts.tecovas.com/authentication/.well-known/jwks.json
  name: shopify-customer-accounts
  response_types:
  - code
  sources:
  - well-known/tecovas-oauth-authorization-server.json
  subject_types:
  - public
  tokenUrl: https://accounts.tecovas.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: tecovas-authentication
source_filename: tecovas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://checkout.tecovas.com/.well-known/oauth-authorization-server\ndocs: https://www.tecovas.com/agents.md\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Tecovas runs two authentication postures. The public read surfaces — the storefront JSON\n    endpoints and the Shopify Storefront GraphQL API — take no credentials at all. The\n    transactional UCP/MCP surface on the checkout host sits in front of Shopify customer\n    accounts, whose OAuth 2.0 / OIDC authorization-server metadata is published anonymously.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://www.tecovas.com/api/productdetail/:slug\n  - https://www.tecovas.com/api/collection\n  - https://www.tecovas.com/api/collection-products\n  - https://www.tecovas.com/api/search-settings\n  - https://checkout.tecovas.com/api/2026-01/graphql.json\n  evidence: >-\n    agents.md states\
  \ \"This site exposes read-only product, collection, and search APIs — no\n    authentication required.\" All four endpoints and GraphQL introspection returned 200\n    anonymously on 2026-08-05.\n- name: ucp-agent-profile\n  type: profile\n  applies_to: [https://checkout.tecovas.com/api/ucp/mcp]\n  parameter: meta.ucp-agent.profile\n  in: request-body\n  required: true\n  description: >-\n    Every UCP MCP tool requires a meta.ucp-agent.profile URI identifying the calling agent.\n    tools/list is anonymous, but an initialize call without a profile returns JSON-RPC error\n    -32001 invalid_profile_url (HTTP 422).\n  evidence: mcp/tecovas-ucp-tools-list.json\n- name: shopify-customer-accounts\n  type: oauth2\n  issuer: https://shopify.com/authentication/9910824\n  authorizationUrl: https://accounts.tecovas.com/authentication/oauth/authorize\n  tokenUrl: https://accounts.tecovas.com/authentication/oauth/token\n  jwks_uri: https://accounts.tecovas.com/authentication/.well-known/jwks.json\n\
  \  end_session_endpoint: https://accounts.tecovas.com/authentication/logout\n  flows:\n  - flow: authorizationCode\n    pkce: [S256]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  response_types: [code]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/tecovas-oauth-authorization-server.json]\nprotected_resource:\n  resource: https://checkout.tecovas.com\n  authorization_servers:\n  - https://accounts.tecovas.com\n  - https://shopify.com/authentication/9910824\n  bearer_methods_supported: [header]\n  source: well-known/tecovas-oauth-protected-resource.json\n  standard: RFC 9728\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://checkout.tecovas.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://checkout.tecovas.com/.well-known/oauth-protected-resource',\
  \ status: 200}\n  - {url: 'https://accounts.tecovas.com/authentication/.well-known/jwks.json', status: 200}\n  - {url: 'https://www.tecovas.com/api/search-settings', status: 200}\n  - {url: 'https://checkout.tecovas.com/api/2026-01/graphql.json', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecovas/refs/heads/main/authentication/tecovas-authentication.yml
summary_line: none/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Footwear
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Product Catalog
---
