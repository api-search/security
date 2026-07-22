---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Duroflexworld Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Duroflexworld secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Duroflexworld
provider_slug: duroflexworld
scheme_count: 2
schemes:
- issuer: https://shopify.com/authentication/38978125956
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://duroflexworld.com/.well-known/openid-configuration
  sources:
  - well-known/duroflexworld-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://account.duroflexworld.com/authentication/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    id_token_alg: RS256
    jwks_uri: https://account.duroflexworld.com/authentication/.well-known/jwks.json
    pkce: S256
    tokenUrl: https://account.duroflexworld.com/authentication/oauth/token
    token_endpoint_auth: client_secret_basic
  name: shopify-customer-account-oauth2
  sources:
  - well-known/duroflexworld-oauth-authorization-server.json
  type: oauth2
slug: duroflexworld-authentication
source_filename: duroflexworld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: well-known/duroflexworld-openid-configuration.json\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: >-\n    Duroflexworld runs on Shopify. Customer authentication uses the Shopify\n    Customer Account API, an OAuth 2.0 / OpenID Connect provider discoverable at\n    the store domain. Storefront browsing (including the Storefront MCP server)\n    is public; authenticated customer operations require an access token from the\n    authorization-code + PKCE flow. There is no first-party developer/partner API\n    program for this store beyond the Shopify platform surfaces.\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://duroflexworld.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/38978125956\n  sources: [well-known/duroflexworld-openid-configuration.json]\n\
  - name: shopify-customer-account-oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.duroflexworld.com/authentication/oauth/authorize\n    tokenUrl: https://account.duroflexworld.com/authentication/oauth/token\n    pkce: S256\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    token_endpoint_auth: client_secret_basic\n    id_token_alg: RS256\n    jwks_uri: https://account.duroflexworld.com/authentication/.well-known/jwks.json\n  sources: [well-known/duroflexworld-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duroflexworld/refs/heads/main/authentication/duroflexworld-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Ecommerce
- Retail
- Sleep
- Mattresses
- Furniture
- Shopify
- MCP
- Consumer Goods
- India
---
