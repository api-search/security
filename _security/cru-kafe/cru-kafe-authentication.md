---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cru Kafe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CRU Kafe declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CRU Kafe
provider_slug: cru-kafe
scheme_count: 1
schemes:
- authorization_endpoint: https://account.crukafe.com/authentication/oauth/authorize
  end_session_endpoint: https://account.crukafe.com/authentication/logout
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify_customer_account_oauth
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/14702456
  jwks_uri: https://account.crukafe.com/authentication/.well-known/jwks.json
  pkce:
    methods:
    - S256
    required: true
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  subject_types:
  - public
  token_endpoint: https://account.crukafe.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: cru-kafe-authentication
source_filename: cru-kafe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.crukafe.com/.well-known/openid-configuration\nsummary: >-\n  CRU Kafe's account surface uses Shopify Customer Account OAuth 2.0 / OpenID Connect\n  (issuer shopify.com/authentication/14702456), Authorization Code with PKCE (S256),\n  RS256-signed ID tokens. This is the Shopify platform identity layer served on the\n  crukafe.com domain, not a bespoke CRU Kafe auth system.\nschemes:\n- id: shopify_customer_account_oauth\n  type: oauth2\n  flow: authorization_code\n  pkce:\n    required: true\n    methods:\n    - S256\n  issuer: https://shopify.com/authentication/14702456\n  authorization_endpoint: https://account.crukafe.com/authentication/oauth/authorize\n  token_endpoint: https://account.crukafe.com/authentication/oauth/token\n  end_session_endpoint: https://account.crukafe.com/authentication/logout\n  jwks_uri: https://account.crukafe.com/authentication/.well-known/jwks.json\n  token_endpoint_auth_methods:\n \
  \ - client_secret_basic\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cru-kafe/refs/heads/main/authentication/cru-kafe-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Coffee
- Ecommerce
- Retail
- Consumer Goods
- Food and Beverage
- Shopify
- Agent Commerce
- UCP
---
