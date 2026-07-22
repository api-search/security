---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: Authentication profile for Urban Revivo's agent/customer-facing surface, captured from the live OIDC discovery and OAuth authorization-server metadata published on the global Shopify storefront (saved verbatim in well-known/). Customer and agent access is brokered by Shopify customer accounts (issuer shopify.com/authentication/50476449942) using OAuth 2.0 authorization-code with PKCE; the UCP MCP shopping endpoint additionally requires an agent profile and buyer-approved checkout.
kind: authentication
layout: security
method: searched
name: Urban Revivo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Urban Revivo secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Urban Revivo
provider_slug: urban-revivo
scheme_count: 1
schemes:
- authorizationUrl: https://shopify.com/authentication/50476449942/oauth/authorize
  issuer: https://shopify.com/authentication/50476449942
  jwksUri: https://shopify.com/authentication/50476449942/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://global.urbanrevivo.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/urban-revivo-openid-configuration.json
  - well-known/urban-revivo-oauth-authorization-server.json
  tokenUrl: https://shopify.com/authentication/50476449942/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: urban-revivo-authentication
source_filename: urban-revivo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://global.urbanrevivo.com/.well-known/openid-configuration\ndescription: >-\n  Authentication profile for Urban Revivo's agent/customer-facing surface,\n  captured from the live OIDC discovery and OAuth authorization-server\n  metadata published on the global Shopify storefront (saved verbatim in\n  well-known/). Customer and agent access is brokered by Shopify customer\n  accounts (issuer shopify.com/authentication/50476449942) using OAuth 2.0\n  authorization-code with PKCE; the UCP MCP shopping endpoint additionally\n  requires an agent profile and buyer-approved checkout.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\nschemes:\n  - name: shopify-customer-accounts-oidc\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/50476449942\n    openIdConnectUrl:\
  \ https://global.urbanrevivo.com/.well-known/openid-configuration\n    authorizationUrl: https://shopify.com/authentication/50476449942/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/50476449942/oauth/token\n    jwksUri: https://shopify.com/authentication/50476449942/.well-known/jwks.json\n    token_endpoint_auth_methods: [client_secret_basic]\n    scopes:\n      - openid\n      - email\n      - customer-account-api:full\n      - customer-account-mcp-api:full\n    sources:\n      - well-known/urban-revivo-openid-configuration.json\n      - well-known/urban-revivo-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-revivo/refs/heads/main/authentication/urban-revivo-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Fashion
- Retail
- eCommerce
- Apparel
- Agentic Commerce
---
