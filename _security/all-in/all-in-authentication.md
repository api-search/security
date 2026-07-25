---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: All In Authentication
name_suffix: Authentication
oauth_flows: []
overview: All In declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: All In
provider_slug: all-in
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/85598339372/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/85598339372/logout
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/85598339372
  jwks_uri: https://shopify.com/authentication/85598339372/.well-known/jwks.json
  pkce: S256
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  standard: OpenID Connect (OIDC)
  token_endpoint: https://shopify.com/authentication/85598339372/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
slug: all-in-authentication
source_filename: all-in-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://allinfood.com/.well-known/openid-configuration + oauth-authorization-server (live)\nhost: allinfood.com\nsummary: >-\n  All In Food's storefront delegates customer identity to Shopify's Customer\n  Account OAuth 2.0 / OpenID Connect authorization server. Agent commerce\n  actions run over the UCP MCP endpoint; end payment is buyer-approved via\n  Shop Pay. No first-party API keys or developer auth are published.\nschemes:\n- type: oauth2\n  flow: authorization_code\n  standard: OpenID Connect (OIDC)\n  issuer: https://shopify.com/authentication/85598339372\n  authorization_endpoint: https://shopify.com/authentication/85598339372/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/85598339372/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/85598339372/logout\n  jwks_uri: https://shopify.com/authentication/85598339372/.well-known/jwks.json\n  pkce: S256\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  id_token_signing_alg:\n  - RS256\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\nnotes:\n- Identity provider is Shopify Customer Accounts, published on the store's own domain via .well-known.\n- The customer-account-mcp-api:full scope authorizes the MCP-based customer/commerce surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/all-in/refs/heads/main/authentication/all-in-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Food
- Snacks
- Nutrition
- Consumer Packaged Goods
- Commerce
- Agent Commerce
- Shopify
- MCP
---
