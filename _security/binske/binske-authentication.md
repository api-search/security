---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Binske Authentication
name_suffix: Authentication
oauth_flows: []
overview: Binske declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Binske
provider_slug: binske
scheme_count: 3
schemes:
- applies_to: https://shopbinske.com/api/ucp/mcp
  name: anonymous
  note: tools/list and catalog reads (search_catalog, lookup_catalog, get_product) answered a 200 with no credentials on 2026-08-07.
  type: none
- authorization_endpoint: https://shopify.com/authentication/64216269035/oauth/authorize
  bearer_methods:
  - header
  end_session_endpoint: https://shopify.com/authentication/64216269035/logout
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/64216269035
  jwks_uri: https://shopify.com/authentication/64216269035/.well-known/jwks.json
  name: shopify_customer_account
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  protected_resource: https://shopbinske.com
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/64216269035/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
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
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/64216269035
  name: openid_connect
  subject_types:
  - public
  type: openIdConnect
slug: binske-authentication
source_filename: binske-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://shopbinske.com/.well-known/oauth-authorization-server\ndocs: https://shopbinske.com/agents.md\nsummary: >-\n  binske publishes no first-party authentication documentation. The one\n  authenticated surface on a binske-controlled host is the Shopify customer\n  account OAuth 2.0 / OpenID Connect stack advertised from the storefront's\n  well-known metadata, plus an anonymous read path on the UCP MCP endpoint.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: https://shopbinske.com/api/ucp/mcp\n  note: >-\n    tools/list and catalog reads (search_catalog, lookup_catalog, get_product)\n    answered a 200 with no credentials on 2026-08-07.\n- name: shopify_customer_account\n  type: oauth2\n  flow: authorization_code\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n  issuer: https://shopify.com/authentication/64216269035\n  authorization_endpoint: https://shopify.com/authentication/64216269035/oauth/authorize\n\
  \  token_endpoint: https://shopify.com/authentication/64216269035/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/64216269035/logout\n  jwks_uri: https://shopify.com/authentication/64216269035/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  bearer_methods: [header]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  protected_resource: https://shopbinske.com\n- name: openid_connect\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/64216269035\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\nbuyer_approval:\n  required_for: [complete_checkout]\n  statement: >-\n    \"Checkout requires human approval. Agents must not complete payment without\n    explicit buyer consent.\"\
  \ — https://shopbinske.com/llms.txt\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://shopbinske.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://shopbinske.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://shopbinske.com/api/ucp/mcp\n    http_status: 200\n    note: anonymous tools/list\nx-gap: >-\n  The authorization server is Shopify's, not binske's. There is no binske\n  developer authentication page, no key issuance, and no first-party token model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binske/refs/heads/main/authentication/binske-authentication.yml
summary_line: 3 schemes
tags:
- Cannabis
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Shopify
- Agent Commerce
- UCP
- MCP
- Storefront
---
