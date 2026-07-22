---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: To The Market Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TO THE MARKET secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TO THE MARKET
provider_slug: to-the-market
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/1239679049/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/1239679049/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/1239679049
  jwks_uri: https://shopify.com/authentication/1239679049/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://tothemarket.com/.well-known/openid-configuration
  pkce_methods:
  - S256
  sources:
  - well-known/to-the-market-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/1239679049/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: to-the-market-authentication
source_filename: to-the-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tothemarket.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Authenticated access to buyer/customer data is via the Shopify Customer\n    Account API using OAuth 2.0 / OpenID Connect (authorization-code flow with\n    PKCE, S256). Read-only catalog browsing over the UCP/MCP surface requires no\n    authentication; checkout completion requires contemporaneous buyer approval.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://tothemarket.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/1239679049\n  authorization_endpoint: https://shopify.com/authentication/1239679049/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/1239679049/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/1239679049/logout\n\
  \  jwks_uri: https://shopify.com/authentication/1239679049/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  pkce_methods:\n  - S256\n  id_token_signing_alg:\n  - RS256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  sources:\n  - well-known/to-the-market-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/to-the-market/refs/heads/main/authentication/to-the-market-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Commerce
- Ecommerce
- Sustainability
- Supply Chain
- Agent Commerce
- Shopify
- MCP
---
