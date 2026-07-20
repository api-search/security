---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crowdmade Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CrowdMade secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CrowdMade
provider_slug: crowdmade
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/17555355/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://shopify.com/authentication/17555355/logout
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/17555355
  jwks_uri: https://shopify.com/authentication/17555355/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://crowdmade.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/crowdmade-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/17555355/oauth/token
  type: openIdConnect
slug: crowdmade-authentication
source_filename: crowdmade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://crowdmade.com/.well-known/openid-configuration\ndocs: https://crowdmade.com/.well-known/oauth-authorization-server\nnotes: >-\n  crowdmade.com is a Shopify-hosted storefront; customer authentication is\n  provided by Shopify Customer Accounts (OpenID Connect). The UCP agent\n  commerce endpoint (/api/ucp/mcp) requires an agent profile URI on discovery\n  and explicit buyer approval at the moment of payment; read-only catalog\n  browsing (products.json, collections/*/products.json, /search) needs no auth.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: S256\n  token_endpoint_auth: client_secret_basic\nschemes:\n  - name: ShopifyCustomerAccountsOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/17555355\n    openIdConnectUrl: https://crowdmade.com/.well-known/openid-configuration\n\
  \    authorization_endpoint: https://shopify.com/authentication/17555355/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/17555355/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/17555355/logout\n    jwks_uri: https://shopify.com/authentication/17555355/.well-known/jwks.json\n    id_token_signing_alg: RS256\n    code_challenge_methods: [S256]\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n    sources: [well-known/crowdmade-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdmade/refs/heads/main/authentication/crowdmade-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Commerce
- E-Commerce
- Merchandise
- Creator Economy
- Shopify
- Agent Commerce
- MCP
- Universal Commerce Protocol
---
