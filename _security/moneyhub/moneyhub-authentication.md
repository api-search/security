---
api_key_in:
- header
api_specs:
- filename: moneyhub-data-api-swagger.json
  format: json
  label: Moneyhub Data & Intelligence API
  slug: moneyhub-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneyhub/refs/heads/main/openapi/moneyhub-data-api-swagger.json
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Moneyhub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- jwt-bearer
overview: Moneyhub secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, and jwt-bearer flow(s).
provider_name: Moneyhub
provider_slug: moneyhub
scheme_count: 3
schemes:
- name: OpenIDConnect
  openIdConnectUrl: https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration
  sources:
  - https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration
  type: openIdConnect
- flows:
  - authorizationUrl: https://identity.moneyhub.co.uk/oidc/auth
    flow: authorizationCode
    tokenUrl: https://identity.moneyhub.co.uk/oidc/token
  - flow: clientCredentials
    tokenUrl: https://identity.moneyhub.co.uk/oidc/token
  name: OAuth2
  sources:
  - https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration
  type: oauth2
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/moneyhub-data-api-swagger.json
  type: apiKey
slug: moneyhub-authentication
source_filename: moneyhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration\ndocs: https://docs.moneyhubenterprise.com/docs/authentication\nnote: >-\n  The Swagger 2.0 Data API declares a Bearer apiKey scheme, but Moneyhub's real\n  authorization surface is a full OpenID Connect / OAuth2 identity layer\n  (node-oidc-provider) at identity.moneyhub.co.uk/oidc, confirmed live from the\n  OIDC discovery document. Access tokens are obtained via authorization_code\n  (data consent), client_credentials (user/admin management) and jwt-bearer\n  grants, then presented as Bearer tokens to the Data API. FAPI-grade options are\n  supported: private_key_jwt and self_signed_tls_client_auth (mTLS) client\n  authentication, Pushed Authorisation Requests (PAR), and signed request objects.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n\
  \  - jwt-bearer\nissuer: https://identity.moneyhub.co.uk/oidc\nendpoints:\n  authorization: https://identity.moneyhub.co.uk/oidc/auth\n  token: https://identity.moneyhub.co.uk/oidc/token\n  jwks: https://identity.moneyhub.co.uk/oidc/certs\n  registration: https://identity.moneyhub.co.uk/oidc/reg\ngrant_types:\n- authorization_code\n- implicit\n- refresh_token\n- client_credentials\n- urn:ietf:params:oauth:grant-type:jwt-bearer\nclient_auth_methods:\n- client_secret_basic\n- private_key_jwt\n- self_signed_tls_client_auth\n- none\nid_token_signing_algs:\n- RS256\n- PS256\n- ES256\n- HS256\nfeatures:\n  pushed_authorisation_requests: true\n  mutual_tls: true\n  request_object_signing: true\n  refresh_tokens: true\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration\n  sources:\n  - https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration\n- name: OAuth2\n  type: oauth2\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: https://identity.moneyhub.co.uk/oidc/auth\n    tokenUrl: https://identity.moneyhub.co.uk/oidc/token\n  - flow: clientCredentials\n    tokenUrl: https://identity.moneyhub.co.uk/oidc/token\n  sources:\n  - https://identity.moneyhub.co.uk/oidc/.well-known/openid-configuration\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/moneyhub-data-api-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneyhub/refs/heads/main/authentication/moneyhub-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Payments
- United Kingdom
- Open Banking
- Open Finance
- Account-to-Account
- Payment Initiation
- Data Aggregation
- AISP
- PISP
- Fintech
---
