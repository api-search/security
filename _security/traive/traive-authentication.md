---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Traive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
- ciba
- password
- implicit
overview: Traive secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, deviceCode, ciba, password, and implicit flow(s).
provider_name: Traive
provider_slug: traive
scheme_count: 1
schemes:
- authorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth
  capabilities:
    ciba: true
    device_authorization_grant: true
    jwt_secured_response_modes: true
    mtls_certificate_bound_access_tokens: true
    pushed_authorization_requests: true
  issuer: https://auth.traive-prod.com/realms/traive-prod
  jwksUri: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/certs
  name: traive-prod
  openIdConnectUrl: https://auth.traive-prod.com/realms/traive-prod/.well-known/openid-configuration
  provider: Keycloak
  sources:
  - well-known/traive-openid-configuration.json
  - well-known/traive-oauth-authorization-server.json
  tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token
  type: openIdConnect
  userinfoUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/userinfo
slug: traive-authentication
source_filename: traive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.traive-prod.com/realms/traive-prod/.well-known/openid-configuration\nnote: Traive publishes no public developer API. This profile documents the platform's\n  authentication surface, harvested from the public OpenID Connect discovery and\n  OAuth 2.0 authorization-server metadata (RFC 8414) of its Keycloak realm\n  traive-prod. Platform login (auth.traive-prod.com) fronts the Traive Agro /\n  Traive Finance applications.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - deviceCode\n  - ciba\n  - password\n  - implicit\n  scopes_supported: 50\nschemes:\n- name: traive-prod\n  type: openIdConnect\n  provider: Keycloak\n  issuer: https://auth.traive-prod.com/realms/traive-prod\n  openIdConnectUrl: https://auth.traive-prod.com/realms/traive-prod/.well-known/openid-configuration\n  authorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth\n\
  \  tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token\n  jwksUri: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/certs\n  userinfoUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/userinfo\n  capabilities:\n    pushed_authorization_requests: true\n    mtls_certificate_bound_access_tokens: true\n    ciba: true\n    device_authorization_grant: true\n    jwt_secured_response_modes: true\n  sources:\n  - well-known/traive-openid-configuration.json\n  - well-known/traive-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traive/refs/heads/main/authentication/traive-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Agriculture
- Fintech
- Credit
- Risk Analysis
- Lending
- AgTech
- Brazil
---
