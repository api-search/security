---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Idme Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ID.me secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ID.me
provider_slug: idme
scheme_count: 3
schemes:
- issuer: https://api.id.me/oidc
  name: OpenIDConnect
  openIdConnectUrl: https://api.id.me/oidc/.well-known/openid-configuration
  sources:
  - well-known/idme-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://api.id.me/oauth/authorize
    flow: authorizationCode
    jwksUrl: https://api.id.me/oidc/.well-known/jwks
    pkce: true
    refresh_token: true
    tokenUrl: https://api.id.me/oauth/token
    userinfoUrl: https://api.id.me/api/public/v3/userinfo
  name: OAuth2
  sources:
  - well-known/idme-openid-configuration.json
  type: oauth2
- applies_to: https://services.idmelabs.com
  description: 'ID.me Services API uses a Base64-encoded account secret sent as "Authorization: Bearer ID.me {token}".'
  name: ServicesApiBearer
  scheme: bearer
  sources:
  - https://docs.id.me/services-api-overview
  type: http
slug: idme-authentication
source_filename: idme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.id.me/guides/oidc/overview\ndocs: https://docs.id.me/guides/open-id-connect/configuration\noidc_issuer: https://api.id.me/oidc\ndiscovery: https://api.id.me/oidc/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.id.me/oidc/.well-known/openid-configuration\n  issuer: https://api.id.me/oidc\n  sources: [well-known/idme-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.id.me/oauth/authorize\n    tokenUrl: https://api.id.me/oauth/token\n    userinfoUrl: https://api.id.me/api/public/v3/userinfo\n    jwksUrl: https://api.id.me/oidc/.well-known/jwks\n    pkce: true\n    refresh_token: true\n  sources:\
  \ [well-known/idme-openid-configuration.json]\n- name: ServicesApiBearer\n  type: http\n  scheme: bearer\n  description: >-\n    ID.me Services API uses a Base64-encoded account secret sent as\n    \"Authorization: Bearer ID.me {token}\".\n  applies_to: https://services.idmelabs.com\n  sources: [https://docs.id.me/services-api-overview]\ntoken_details:\n  id_token_signing_alg: [RS256, ES256]\n  id_token_encryption_alg: [RSA-OAEP]\n  id_token_encryption_enc: [A256CBC-HS512]\n  userinfo_signing_alg: [RS256, ES256]\nnotes: >-\n  Also supports SAML 2.0 federation for IAM platforms (Okta, Keycloak, Microsoft\n  Entra External ID, PingOne, AWS Cognito). See docs.id.me/guides/saml/overview.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/authentication/idme-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Identity
- Identity Verification
- Authentication
- OpenID Connect
- OAuth 2.0
- SAML
- Single Sign-On
- Digital Identity
- KYC
- Fraud Prevention
- Government
---
