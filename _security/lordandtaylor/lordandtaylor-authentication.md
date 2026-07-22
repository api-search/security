---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Lordandtaylor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lord & Taylor secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lord & Taylor
provider_slug: lordandtaylor
scheme_count: 2
schemes:
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/90637893921
  jwks_uri: https://account.lordandtaylor.com/authentication/.well-known/jwks.json
  name: oidc
  openid_configuration: https://www.lordandtaylor.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
- flows:
  - authorizationUrl: https://account.lordandtaylor.com/authentication/oauth/authorize
    code_challenge_methods_supported:
    - S256
    end_session_endpoint: https://account.lordandtaylor.com/authentication/logout
    flow: authorizationCode
    grant_types_supported:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://account.lordandtaylor.com/authentication/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_basic
  name: oauth2
  type: oauth2
slug: lordandtaylor-authentication
source_filename: lordandtaylor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.lordandtaylor.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  provider: Shopify Customer Accounts\nschemes:\n- name: oidc\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/90637893921\n  openid_configuration: https://www.lordandtaylor.com/.well-known/openid-configuration\n  jwks_uri: https://account.lordandtaylor.com/authentication/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.lordandtaylor.com/authentication/oauth/authorize\n    tokenUrl: https://account.lordandtaylor.com/authentication/oauth/token\n    end_session_endpoint:\
  \ https://account.lordandtaylor.com/authentication/logout\n    code_challenge_methods_supported: [S256]\n    grant_types_supported:\n    - authorization_code\n    - refresh_token\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    scopes: [openid, email, customer-account-api:full, customer-account-mcp-api:full]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lordandtaylor/refs/heads/main/authentication/lordandtaylor-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Shopping
- Department Store
- Agentic Commerce
- MCP
---
