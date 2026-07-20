---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Infinite Athlete Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Infinite Athlete secures its APIs with apiKey, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Infinite Athlete
provider_slug: infinite-athlete
scheme_count: 5
schemes:
- description: Long-lived FusionFeed API key sent in the Authorization header using the "token" scheme. Issued by FusionFeed to invited clients.
  format: 'Authorization: token MY_API_KEY_TOKEN'
  header: Authorization
  in: header
  name: ApiKeyToken
  source: https://docs.tempus-ex.com/fusionfeed/authentication
  type: apiKey
- bearerFormat: JWT
  description: JSON Web Token presented as an RFC 6750 bearer token. FusionFeed validates the JWT; tokens are minted by an external identity provider, not by FusionFeed.
  format: 'Authorization: Bearer [example key]'
  name: BearerJWT
  scheme: bearer
  source: https://docs.tempus-ex.com/fusionfeed/authentication
  type: http
- authorizationUrl: https://tempus-ex.okta.com/oauth2/v1/authorize
  description: OAuth2 Authorization Code flow with PKCE via Tempus Ex's Okta tenant. Requires a client ID and redirect URI. The resulting ID/access token is presented to FusionFeed as a bearer JWT.
  flow: authorizationCode
  issuer: https://tempus-ex.okta.com
  name: OktaOAuth2
  pkce: true
  provider: okta
  scopes_requested:
  - openid
  - profile
  - email
  source: https://docs.tempus-ex.com/fusionfeed/authentication
  tokenUrl: https://tempus-ex.okta.com/oauth2/v1/token
  type: oauth2
- description: Amazon Cognito as an alternative identity provider using the USER_PASSWORD_AUTH flow (client ID + username + password, e.g. via the AWS CLI cognito-idp initiate-auth). The returned JWT is presented to FusionFeed as a bearer token.
  flow: USER_PASSWORD_AUTH
  name: CognitoOAuth2
  provider: cognito
  source: https://docs.tempus-ex.com/fusionfeed/authentication
  type: oauth2
- description: Organizations may run their own JWT server and embed access-control policies in tokens for their users; FusionFeed validates these as bearer JWTs.
  name: CustomJWT
  provider: custom
  source: https://docs.tempus-ex.com/fusionfeed/authentication
  type: openIdConnect
slug: infinite-athlete-authentication
source_filename: infinite-athlete-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.tempus-ex.com/fusionfeed/authentication\napi: FusionFeed\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  api_key_header: Authorization\n  api_key_scheme: token\n  http_bearer: true\n  oauth2_flows: [authorizationCode]\n  identity_providers: [okta, cognito, custom]\n  note: >-\n    FusionFeed is a resource server. JWTs are not issued by FusionFeed itself; it\n    validates bearer tokens minted by an external identity provider (Okta, Amazon\n    Cognito, or a custom JWT server with embedded access-control policies).\nschemes:\n- name: ApiKeyToken\n  type: apiKey\n  in: header\n  header: Authorization\n  format: 'Authorization: token MY_API_KEY_TOKEN'\n  description: >-\n    Long-lived FusionFeed API key sent in the Authorization header using the\n    \"token\" scheme. Issued by FusionFeed to invited clients.\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n- name:\
  \ BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  format: 'Authorization: Bearer [example key]'\n  description: >-\n    JSON Web Token presented as an RFC 6750 bearer token. FusionFeed validates the\n    JWT; tokens are minted by an external identity provider, not by FusionFeed.\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n- name: OktaOAuth2\n  type: oauth2\n  provider: okta\n  flow: authorizationCode\n  pkce: true\n  issuer: https://tempus-ex.okta.com\n  authorizationUrl: https://tempus-ex.okta.com/oauth2/v1/authorize\n  tokenUrl: https://tempus-ex.okta.com/oauth2/v1/token\n  scopes_requested: [openid, profile, email]\n  description: >-\n    OAuth2 Authorization Code flow with PKCE via Tempus Ex's Okta tenant. Requires\n    a client ID and redirect URI. The resulting ID/access token is presented to\n    FusionFeed as a bearer JWT.\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n- name: CognitoOAuth2\n  type: oauth2\n  provider: cognito\n\
  \  flow: USER_PASSWORD_AUTH\n  description: >-\n    Amazon Cognito as an alternative identity provider using the USER_PASSWORD_AUTH\n    flow (client ID + username + password, e.g. via the AWS CLI\n    cognito-idp initiate-auth). The returned JWT is presented to FusionFeed as a\n    bearer token.\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n- name: CustomJWT\n  type: openIdConnect\n  provider: custom\n  description: >-\n    Organizations may run their own JWT server and embed access-control policies in\n    tokens for their users; FusionFeed validates these as bearer JWTs.\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinite-athlete/refs/heads/main/authentication/infinite-athlete-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Sports
- Sports Technology
- Sports Data
- Athlete Performance
- Biomechanics
- Video
- Real-Time Data
- Analytics
- GraphQL
---
