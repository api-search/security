---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Primary Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Primary secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Primary
provider_slug: primary
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/30430134331/oauth/authorize
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/30430134331
  jwks_uri: https://shopify.com/authentication/30430134331/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  pkce: true
  sources:
  - well-known/primary-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/30430134331/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: primary-authentication
source_filename: primary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://www.primary.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server (Shopify Customer Account API discovery)\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  notes: >-\n    primary.com is a Shopify storefront; buyer-facing authentication is handled by\n    Shopify's Customer Account API (OAuth2 + OIDC). No first-party API of Primary's\n    own — the storefront exposes an open MCP server for catalog/cart plus this\n    OAuth2/OIDC surface for customer-scoped operations.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/30430134331\n  authorization_endpoint: https://shopify.com/authentication/30430134331/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/30430134331/oauth/token\n\
  \  jwks_uri: https://shopify.com/authentication/30430134331/.well-known/jwks.json\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  pkce: true\n  sources: [well-known/primary-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primary/refs/heads/main/authentication/primary-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Retail
- Ecommerce
- Apparel
- Children
- Shopify
- Agent
---
