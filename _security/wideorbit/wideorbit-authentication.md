---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Wideorbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: WideOrbit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: WideOrbit
provider_slug: wideorbit
scheme_count: 1
schemes:
- endpoints:
    authorization: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/auth
    jwks: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/certs
    token: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/token
  environments:
    pre-production: https://ppe-sso.wocentral.com/auth/realms/externalgateway
    production: https://sso.wocentral.com/auth/realms/externalgateway
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  id: oidc_externalgateway
  issuer: https://sso.wocentral.com/auth/realms/externalgateway
  observed_default_scope: openid
  observed_gateway_client: apigateway
  openIdConnectUrl: https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration
  provider: Keycloak (WO Central)
  realm: externalgateway
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
slug: wideorbit-authentication
source_filename: wideorbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  WO Central Keycloak OIDC discovery document\n  (https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration)\n  observed live redirect from https://apigateway.wideorbit.com\ndocs: https://www.wideorbit.com/io/\nsummary: >-\n  The WideOrbit.io partner API gateway is protected by OpenID Connect on a\n  Keycloak identity provider hosted at WO Central. Every unauthenticated request\n  to apigateway.wideorbit.com is redirected to the \"externalgateway\" realm\n  authorization endpoint (client_id=apigateway, scope=openid, response_type=code),\n  confirming the OAuth 2.0 authorization-code flow. The realm also advertises\n  client_credentials for machine-to-machine partner integrations.\nschemes:\n- id: oidc_externalgateway\n  type: openIdConnect\n  provider: Keycloak (WO Central)\n  realm: externalgateway\n  openIdConnectUrl: https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration\n\
  \  issuer: https://sso.wocentral.com/auth/realms/externalgateway\n  endpoints:\n    authorization: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/auth\n    token: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/token\n    jwks: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/certs\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  observed_gateway_client: apigateway\n  observed_default_scope: openid\n  environments:\n    production: https://sso.wocentral.com/auth/realms/externalgateway\n    pre-production: https://ppe-sso.wocentral.com/auth/realms/externalgateway\nnotes: >-\n  Access is limited to WideOrbit-certified partners; credentials are\
  \ provisioned\n  through the WideOrbit.io program rather than self-service registration. No\n  API-key or HTTP-basic scheme was observed on the gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideorbit/refs/heads/main/authentication/wideorbit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Advertising
- AdTech
- Media
- Broadcasting
- Radio
- Television
- Ad Management
- Programmatic
- Media Sales
---
