---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Thamarah Al Jill Co Llc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Thamarah Al-Jill Co LLC secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Thamarah Al-Jill Co LLC
provider_slug: thamarah-al-jill-co-llc
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/29798400044/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/29798400044/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/29798400044
  jwks_uri: https://shopify.com/authentication/29798400044/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  response_types_supported:
  - code
  sources:
  - well-known/thamarah-al-jill-co-llc-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/29798400044/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: thamarah-al-jill-co-llc-authentication
source_filename: thamarah-al-jill-co-llc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://amusedco.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  provider: Shopify Customer Accounts\nnotes: >-\n  Buyer/customer authentication is delegated to Shopify Customer Accounts. The store's\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server both\n  resolve to the Shopify-hosted issuer below. Agent-driven checkout via the UCP MCP\n  surface additionally enforces a buyer-approval invariant at the moment of payment\n  (see conventions/). No custom first-party auth scheme is published by the merchant.\nschemes:\n  - name: shopify-customer-accounts-oidc\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/29798400044\n    authorization_endpoint: https://shopify.com/authentication/29798400044/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/29798400044/oauth/token\n    end_session_endpoint:\
  \ https://shopify.com/authentication/29798400044/logout\n    jwks_uri: https://shopify.com/authentication/29798400044/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    code_challenge_methods_supported: [S256]     # PKCE\n    subject_types_supported: [public]\n    sources:\n      - well-known/thamarah-al-jill-co-llc-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thamarah-al-jill-co-llc/refs/heads/main/authentication/thamarah-al-jill-co-llc-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- E-commerce
- Marketplace
- Luxury
- Resale
- Fashion
- Agent Commerce
- Shopify
- Saudi Arabia
---
