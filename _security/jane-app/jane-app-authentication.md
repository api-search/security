---
api_key_in: []
api_specs:
- filename: jane-app-jdp-openapi.yml
  format: yaml
  label: Jane JDP API
  slug: jane-app-jdp-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-jdp-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jane App Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jane secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jane
provider_slug: jane-app
scheme_count: 2
schemes:
- description: 'OAuth2 authorization code flow with PKCE (Proof Key for Code Exchange) support.


    **PKCE Flow Required**: All integrations must use PKCE flow for authentication.


    **PKCE Benefits:**

    - Enhanced security against authorization code interception attacks

    - S256 code challenge method supported

    - Industry best practice for OAuth2 implementations


    **Implementation**: Use the authorization code flow with PK'
  flows:
  - authorizationUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/auth?response_type=code&resource=https://jdpdocsdemo.jane.qa&prompt=consent
    flow: authorizationCode
    scopes: 27
    tokenUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/jane-app-jdp-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/jane-app-jdp-openapi.yml
  type: http
slug: jane-app-authentication
source_filename: jane-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/jane-app-jdp-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: required (S256)\n  identity_provider: Keycloak\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/auth?response_type=code&resource=https://jdpdocsdemo.jane.qa&prompt=consent\n    tokenUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token\n    scopes: 27\n  description: 'OAuth2 authorization code flow with PKCE (Proof Key for Code Exchange) support.\n\n\n    **PKCE Flow Required**: All integrations must use PKCE flow for authentication.\n\n\n    **PKCE Benefits:**\n\n    - Enhanced security against authorization code interception attacks\n\n    - S256 code challenge method supported\n\n    - Industry best practice for OAuth2 implementations\n\
  \n\n    **Implementation**: Use the authorization code flow with PK'\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\ndocs: https://developers.jane.app/docs/getting-started\noidc_discovery:\n  production: https://login.id.janeapp.com/realms/jane/.well-known/openid-configuration\n  sandbox: https://login.id.janeapp.com/realms/jane_partner_sandbox/.well-known/openid-configuration\n  oauth_authorization_server: https://login.id.janeapp.com/realms/jane/.well-known/oauth-authorization-server\n  saved:\n  - well-known/jane-app-prod-openid-configuration.json\n  - well-known/jane-app-sandbox-openid-configuration.json\n  - well-known/jane-app-oauth-authorization-server.json\nendpoints:\n  authorization: https://login.id.janeapp.com/realms/{realm}/protocol/openid-connect/auth\n  token: https://login.id.janeapp.com/realms/{realm}/protocol/openid-connect/token\n  introspection:\
  \ https://login.id.janeapp.com/realms/{realm}/protocol/openid-connect/token/introspect\n  revocation: https://login.id.janeapp.com/realms/{realm}/protocol/openid-connect/revoke\n  jwks: https://login.id.janeapp.com/realms/{realm}/protocol/openid-connect/certs\n  realms:\n    production: jane\n    sandbox: jane_partner_sandbox\ntokens:\n  format: RS256-signed JWT\n  type: Bearer\n  access_token_ttl: 300s (5 min)\n  refresh_token_ttl: 1800s (30 min)\n  code_challenge_methods:\n  - S256\n  claims:\n  - exp\n  - iat\n  - jti\n  - iss\n  - aud\n  - sub\n  - azp\n  - resource_access\n  - resource_owner\n  - scope\nnote: OAuth 2.0 Authorization Code + PKCE over OIDC (Keycloak). BearerAuth (http/bearer JWT) is the resource-server\n  token presentation. Not SMART-on-FHIR.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/authentication/jane-app-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- Canada
- Practice Management
- EHR
- EMR
- Scheduling
- Clinical Documentation
- Telehealth
- Health and Wellness
- REST API
- Authentication
- Webhook
---
