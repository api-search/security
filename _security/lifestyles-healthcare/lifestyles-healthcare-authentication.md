---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lifestyles Healthcare Authentication
name_suffix: Authentication
oauth_flows: []
overview: LifeStyles Healthcare declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: LifeStyles Healthcare
provider_slug: lifestyles-healthcare
scheme_count: 3
schemes:
- applies_to: Read-only storefront JSON (/products.json, /collections/{handle}/products.json, /products/{handle}.json, /search, /cart.js, /sitemap.xml).
  evidence: https://lifestyles.com/llms.txt
  name: none
  type: none
- authorization_endpoint: https://shopify.com/authentication/61038100706/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/61038100706/logout
  evidence: https://lifestyles.com/.well-known/openid-configuration
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/61038100706
  jwks_uri: https://shopify.com/authentication/61038100706/.well-known/jwks.json
  name: shopify_customer_accounts
  openIdConnectUrl: https://lifestyles.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  token_endpoint: https://shopify.com/authentication/61038100706/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to: https://lifestyles.com/api/ucp/mcp
  description: The UCP MCP endpoint requires the calling agent to present a profile URI. Calls without one are rejected with JSON-RPC error -32001 (invalid_profile_url).
  evidence: probed 2026-07-19 - POST https://lifestyles.com/api/ucp/mcp tools/list
  name: ucp_agent_profile
  type: agentProfile
slug: lifestyles-healthcare-authentication
source_filename: lifestyles-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://lifestyles.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary: >-\n  The LifeStyles US storefront exposes two access modes: unauthenticated read-only\n  browsing of catalog JSON endpoints, and Shopify Customer Accounts OpenID Connect for\n  buyer-scoped access. Agent commerce over the UCP MCP endpoint additionally requires an\n  agent profile URI and explicit buyer approval at payment.\nschemes:\n- name: none\n  type: none\n  applies_to: >-\n    Read-only storefront JSON (/products.json, /collections/{handle}/products.json,\n    /products/{handle}.json, /search, /cart.js, /sitemap.xml).\n  evidence: https://lifestyles.com/llms.txt\n- name: shopify_customer_accounts\n  type: openIdConnect\n  openIdConnectUrl: https://lifestyles.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/61038100706\n  authorization_endpoint: https://shopify.com/authentication/61038100706/oauth/authorize\n\
  \  token_endpoint: https://shopify.com/authentication/61038100706/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/61038100706/logout\n  jwks_uri: https://shopify.com/authentication/61038100706/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  evidence: https://lifestyles.com/.well-known/openid-configuration\n- name: ucp_agent_profile\n  type: agentProfile\n  applies_to: https://lifestyles.com/api/ucp/mcp\n  description: >-\n    The UCP MCP endpoint requires\
  \ the calling agent to present a profile URI. Calls\n    without one are rejected with JSON-RPC error -32001 (invalid_profile_url).\n  evidence: probed 2026-07-19 - POST https://lifestyles.com/api/ucp/mcp tools/list\nobservations:\n  probed: '2026-07-19'\n  security_txt: absent (404 at /.well-known/security.txt)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifestyles-healthcare/refs/heads/main/authentication/lifestyles-healthcare-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Healthcare
- Sexual Wellness
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- MCP
- Shopify
- Retail
---
