---
api_key_in:
- header
api_specs:
- filename: tempus-ex-fusionfeed-asyncapi.yml
  format: yaml
  label: FusionFeed
  slug: fusionfeed
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tempus-ex/refs/heads/main/asyncapi/tempus-ex-fusionfeed-asyncapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Tempus Ex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tempus Ex secures its APIs with apiKey, http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tempus Ex
provider_slug: tempus-ex
scheme_count: 2
schemes:
- description: 'Long-lived API key issued by Tempus Ex, presented as "Authorization: token MY_API_KEY_TOKEN". For WebSocket (graphql-ws) connections the key is passed in the connection-init parameters as {"authorization": "token MY_API_KEY"} since browsers cannot set WS headers.'
  format: token <API_KEY>
  in: header
  name: apiKeyToken
  parameter: Authorization
  sources:
  - docs
  type: apiKey
- bearerFormat: JWT
  description: 'JSON Web Token issued by an external identity provider, presented as "Authorization: Bearer MY_JWT_TOKEN". FusionFeed acts as an OAuth2 resource server that validates the token.'
  format: Bearer <JWT>
  in: header
  name: bearerJWT
  parameter: Authorization
  scheme: bearer
  sources:
  - docs
  type: http
slug: tempus-ex-authentication
source_filename: tempus-ex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tempus-ex.com/fusionfeed/authentication\ndocs: https://docs.tempus-ex.com/fusionfeed/authentication\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    FusionFeed authenticates in two ways: a long-lived API key sent via the\n    \"Authorization: token\" HTTP header, or a JWT sent via the\n    \"Authorization: Bearer\" header. FusionFeed is an OAuth2 resource server —\n    it does NOT mint JWTs; an external identity provider (Okta, Amazon Cognito,\n    or a customer's own IdP) issues the tokens. Access-control policies can be\n    embedded directly in the JWT claims for fine-grained, per-user access.\nschemes:\n- name: apiKeyToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'token <API_KEY>'\n  description: >-\n    Long-lived API key issued by Tempus Ex, presented as\n    \"Authorization: token MY_API_KEY_TOKEN\"\
  . For WebSocket (graphql-ws)\n    connections the key is passed in the connection-init parameters as\n    {\"authorization\": \"token MY_API_KEY\"} since browsers cannot set WS headers.\n  sources: [docs]\n- name: bearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  format: 'Bearer <JWT>'\n  description: >-\n    JSON Web Token issued by an external identity provider, presented as\n    \"Authorization: Bearer MY_JWT_TOKEN\". FusionFeed acts as an OAuth2 resource\n    server that validates the token.\n  sources: [docs]\nidentity_providers:\n- name: Okta\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  scopes: [openid, profile, email]\n  authorizationUrl: https://tempus-ex.okta.com/oauth2/v1/authorize\n  tokenUrl: https://tempus-ex.okta.com/oauth2/v1/token\n  description: >-\n    Standard OAuth2 authorization-code-with-PKCE flow against Tempus Ex's Okta\n    tenant; the returned id token is used as the FusionFeed Bearer JWT.\n\
  - name: Amazon Cognito\n  type: oauth2\n  flow: USER_PASSWORD_AUTH\n  region: us-east-1\n  description: >-\n    Cognito user-pool authentication (initiate-auth USER_PASSWORD_AUTH); the\n    returned id token is used as the FusionFeed Bearer JWT.\n- name: Custom Identity Provider\n  type: openIdConnect\n  description: >-\n    Customers may run their own IdP to mint JWTs for their end users, embedding\n    fine-grained access-control policies in the token claims so users can call\n    FusionFeed directly. Contact support to enable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempus-ex/refs/heads/main/authentication/tempus-ex-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Sports Data
- Sports
- Video
- Streaming
- Telemetry
- GraphQL
- REST
- Media
- NFL
- Analytics
---
