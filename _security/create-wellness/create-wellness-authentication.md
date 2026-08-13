---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Create Wellness Authentication
name_suffix: Authentication
oauth_flows: []
overview: Create Wellness declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Create Wellness
provider_slug: create-wellness
scheme_count: 0
schemes: []
slug: create-wellness-authentication
source_filename: create-wellness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://trycreate.co/.well-known/openid-configuration\ndocs: https://trycreate.co/llms.txt\nnote: >-\n  Derived from the live /.well-known/ documents served on trycreate.co plus the\n  observed behaviour of the UCP MCP endpoint. There is no OpenAPI to derive\n  securitySchemes from; every statement below was read off a document that\n  returned 200 on 2026-08-11.\nsurfaces:\n- surface: UCP Commerce MCP\n  url: https://trycreate.co/api/ucp/mcp\n  scheme: none\n  anonymous: true\n  evidence: >-\n    POST tools/list with no Authorization header returned 200 and the full\n    13-tool manifest. No WWW-Authenticate challenge, no invalid_token error.\n  identity_input:\n    field: meta[\"ucp-agent\"].profile\n    type: uri\n    required: true\n    description: >-\n      Every tool requires an agent profile URI in meta. This is agent\n      self-identification for UCP discovery, not authentication — it is not\n      verified against\
  \ any credential.\n  human_in_the_loop:\n    required_for: complete_checkout\n    statement: >-\n      \"Checkout requires human approval. Agents must not complete payment\n      without explicit buyer consent.\" (llms.txt / robots.txt)\n- surface: Shopify Customer Accounts\n  scheme: openIdConnect\n  type: oauth2\n  issuer: https://shopify.com/authentication/61192044732\n  discovery: https://trycreate.co/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/61192044732/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/61192044732/oauth/token\n  jwks_uri: https://shopify.com/authentication/61192044732/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/61192044732/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  id_token_signing_alg:\n  - RS256\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  human_login: https://trycreate.co/account/login\nprotected_resource:\n  source: https://trycreate.co/.well-known/oauth-protected-resource\n  resource: https://trycreate.co\n  authorization_servers:\n  - https://shopify.com/authentication/61192044732\n  bearer_methods_supported:\n  - header\ngaps:\n- >-\n  The authorization server is Shopify's, not Create Wellness's — a buyer\n  authenticating against this store is authenticating against\n  shopify.com/authentication/61192044732. There is no brand-operated IdP.\n- >-\n  No published API key programme, no partner/developer credential, and no\n  developer documentation of any kind on the brand host. The only auth\n  documentation is the platform-generated llms.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/create-wellness/refs/heads/main/authentication/create-wellness-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health and Wellness
- Supplements
- Consumer Products
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- MCP
- Shopify
- Nutrition
---
