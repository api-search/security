---
api_key_in: []
api_specs:
- filename: versapay-api-reference.json
  format: json
  label: Versapay API Reference
  slug: versapay-api-reference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/openapi/versapay-api-reference.json
- filename: versapay-ecommerce-api.json
  format: json
  label: Versapay Ecommerce API
  slug: versapay-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/openapi/versapay-ecommerce-api.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Versapay Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
overview: Versapay secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and password flow(s).
provider_name: Versapay
provider_slug: versapay
scheme_count: 4
schemes:
- description: 'Primary API auth. HTTPS Basic access authentication supplying the account''s API Token as the username and API Key as the password (curl -u "Token:Key"). Credentials are generated/disabled in the account console at https://secure.versapay.com/account (UAT: https://uat.versapay.com/account).'
  name: apiTokenKeyBasic
  scheme: basic
  sources:
  - https://developers.versapay.com/
  type: http
- bearerFormat: JWT
  description: Alternative auth via HTTPS Bearer authentication with a JWT token.
  name: jwtBearer
  scheme: bearer
  sources:
  - https://developers.versapay.com/
  type: http
- description: 'Doorkeeper OAuth2/OIDC server on secure.versapay.com. Scopes: receivables, payables, read, write, update.'
  flows:
    authorizationCode:
      authorizationUrl: https://secure.versapay.com/oauth/authorize
      scopes:
      - receivables
      - payables
      - read
      - write
      - update
      tokenUrl: https://secure.versapay.com/oauth/token
    clientCredentials:
      scopes:
      - receivables
      - payables
      - read
      - write
      - update
      tokenUrl: https://secure.versapay.com/oauth/token
    password:
      scopes:
      - receivables
      - payables
      - read
      - write
      - update
      tokenUrl: https://secure.versapay.com/oauth/token
  name: oauth2
  sources:
  - https://secure.versapay.com/.well-known/openid-configuration
  type: oauth2
- description: OIDC discovery available; id_token signed RS256, userinfo + jwks endpoints published.
  name: openIdConnect
  openIdConnectUrl: https://secure.versapay.com/.well-known/openid-configuration
  sources:
  - https://secure.versapay.com/.well-known/openid-configuration
  type: openIdConnect
slug: versapay-authentication
source_filename: versapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developers.versapay.com/\ndocs: https://developers.versapay.com/\nnotes: >-\n  The published OpenAPI specs do not declare components.securitySchemes, so this\n  profile is searched from the docs Authentication section plus the live OAuth/OIDC\n  discovery document at secure.versapay.com/.well-known/openid-configuration.\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, password]\nschemes:\n  - name: apiTokenKeyBasic\n    type: http\n    scheme: basic\n    description: >-\n      Primary API auth. HTTPS Basic access authentication supplying the account's\n      API Token as the username and API Key as the password (curl -u \"Token:Key\").\n      Credentials are generated/disabled in the account console at\n      https://secure.versapay.com/account (UAT: https://uat.versapay.com/account).\n    sources: [https://developers.versapay.com/]\n\
  \  - name: jwtBearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Alternative auth via HTTPS Bearer authentication with a JWT token.\n    sources: [https://developers.versapay.com/]\n  - name: oauth2\n    type: oauth2\n    description: >-\n      Doorkeeper OAuth2/OIDC server on secure.versapay.com. Scopes: receivables,\n      payables, read, write, update.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://secure.versapay.com/oauth/authorize\n        tokenUrl: https://secure.versapay.com/oauth/token\n        scopes: [receivables, payables, read, write, update]\n      clientCredentials:\n        tokenUrl: https://secure.versapay.com/oauth/token\n        scopes: [receivables, payables, read, write, update]\n      password:\n        tokenUrl: https://secure.versapay.com/oauth/token\n        scopes: [receivables, payables, read, write, update]\n    sources: [https://secure.versapay.com/.well-known/openid-configuration]\n  - name: openIdConnect\n\
  \    type: openIdConnect\n    openIdConnectUrl: https://secure.versapay.com/.well-known/openid-configuration\n    description: OIDC discovery available; id_token signed RS256, userinfo + jwks endpoints published.\n    sources: [https://secure.versapay.com/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versapay/refs/heads/main/authentication/versapay-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Payments
- Canada
- Accounts Receivable
- AR Automation
- Order to Cash
- Payment Acceptance
- Payment Processing
- B2B Payments
- Invoicing
- Ecommerce
- Card Present
- Webhooks
---
