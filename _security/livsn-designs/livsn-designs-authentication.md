---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Livsn Designs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Livsn Designs secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Livsn Designs
provider_slug: livsn-designs
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/27194140/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/27194140/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/27194140
  jwks_uri: https://shopify.com/authentication/27194140/.well-known/jwks.json
  name: shopify-customer-account
  provider: Shopify
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/livsn-designs-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/27194140/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: livsn-designs-authentication
source_filename: livsn-designs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.livsndesigns.com/.well-known/openid-configuration\nnotes: >-\n  Livsn Designs publishes no first-party API, so there is no bespoke auth model.\n  The only authentication surface on the domain is the Shopify Customer Account\n  API OIDC/OAuth2 authorization server that Shopify serves per-merchant. Captured\n  verbatim from the merchant-scoped discovery document (issuer 27194140).\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  provider: Shopify Customer Account API\nschemes:\n  - name: shopify-customer-account\n    type: openIdConnect\n    provider: Shopify\n    issuer: https://shopify.com/authentication/27194140\n    authorization_endpoint: https://shopify.com/authentication/27194140/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/27194140/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/27194140/logout\n    jwks_uri: https://shopify.com/authentication/27194140/.well-known/jwks.json\n\
  \    grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    response_types_supported: [code]\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic]\n    scopes_supported:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    source: well-known/livsn-designs-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livsn-designs/refs/heads/main/authentication/livsn-designs-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Retail
- E-commerce
- Apparel
- Outdoor
- Shopify
- Agent Commerce
- UCP
- MCP
---
