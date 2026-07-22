---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Jubilee Tv Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jubilee TV secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jubilee TV
provider_slug: jubilee-tv
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/83104301340/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/83104301340/logout
  issuer: https://shopify.com/authentication/83104301340
  jwks_uri: https://shopify.com/authentication/83104301340/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/jubilee-tv-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/83104301340/oauth/token
  type: openIdConnect
slug: jubilee-tv-authentication
source_filename: jubilee-tv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://getjubileetv.com/.well-known/openid-configuration\ndocs: https://getjubileetv.com/.well-known/oauth-authorization-server\nnotes: >-\n  Authentication is Shopify Customer Accounts (OpenID Connect / OAuth 2.0),\n  provided by the commerce platform for the getjubileetv.com storefront. There is\n  no bespoke Jubilee TV developer API key or token program published. The\n  authorization server is issued under shopify.com/authentication/83104301340.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/83104301340\n  authorization_endpoint: https://shopify.com/authentication/83104301340/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/83104301340/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/83104301340/logout\n  jwks_uri: https://shopify.com/authentication/83104301340/.well-known/jwks.json\n  response_types_supported: [code]\n  scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/jubilee-tv-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jubilee-tv/refs/heads/main/authentication/jubilee-tv-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Consumer
- Caregiving
- Seniors
- Smart TV
- Video Calling
- Agentic Commerce
- Shopify
---
