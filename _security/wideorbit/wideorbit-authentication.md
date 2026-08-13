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
overview: WideOrbit declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: WideOrbit
provider_slug: wideorbit
scheme_count: 3
schemes:
- applies_to: WideOrbit.io API Gateway (https://apigateway.wideorbit.com)
  endpoints:
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
- applies_to: WO Data API (DAPI) 4.2.1
  callback_subset:
    note: The integrator's callback acknowledgement POST to {root}/api/Requests/Update/{requestId} carries only partner-id and api-key — agreement-key is not required on that call.
  failure:
    body: '{ "Error": "Unauthorized access" }'
    note: Returned when no valid combination is found. Authentication and authorization failures are not distinguished.
    status: 401
  id: wo_data_api_header_keys
  in: header
  model: closed
  model_note: '"DAPI uses the closed authentication model, where client authentication and usage patterns are managed by WideOrbit." Credentials are provisioned by WideOrbit Support; there is no registration endpoint, no token exchange, no expiry and no rotation procedure documented.'
  names:
  - description: Identifies the certified software provider calling the API.
    name: partner-id
    required: true
  - description: The secret issued to that partner.
    name: api-key
    required: true
  - description: Identifies the contractual data area. "Each combination uniquely identifies the area of WO Network, WO Traffic, or WO Omni data to be accessed and the API client requesting access." This header is the tenancy boundary.
    name: agreement-key
    required: true
  source: '"WO Data API uses HTTP request header information to authorize requests and authenticate users." — WO Data API Guide 4.2.1, Authentication'
  transport: HTTPS ("We do recommend, always use HTTPS secure endpoint.")
  type: apiKey
- applies_to: '{root}/api/Diagnostic/status_check'
  id: wo_data_api_diagnostic_key
  in: header
  names:
  - description: A separate GUID-shaped key guarding the broadcaster connection health check. Does not use the partner/api/agreement triple.
    name: DiagnosticSecurityKey
    required: true
  type: apiKey
slug: wideorbit-authentication
source_filename: wideorbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  WO Central Keycloak OIDC discovery document\n  (https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration)\n  observed live redirect from https://apigateway.wideorbit.com; plus the\n  Authentication section of the WO Data API Guide 4.2.1\n  (https://www.wideorbit.com/wp-content/uploads/2022/07/WO-DATA-API-Guide-Version-421_New.pdf)\ndocs: https://www.wideorbit.com/io/\nsummary: >-\n  WideOrbit runs two independent authentication models across two API surfaces.\n  The WideOrbit.io partner API gateway is protected by OpenID Connect on a\n  Keycloak identity provider hosted at WO Central. Every unauthenticated request\n  to apigateway.wideorbit.com is redirected to the \"externalgateway\" realm\n  authorization endpoint (client_id=apigateway, scope=openid, response_type=code),\n  confirming the OAuth 2.0 authorization-code flow. The realm also advertises\n  client_credentials for machine-to-machine\
  \ partner integrations. The separately\n  documented WO Data API does NOT use that identity provider at all — it\n  authenticates on three flat request headers issued out of band by WideOrbit\n  Support, with a fourth header guarding the diagnostic endpoint. Neither\n  surface offers self-service registration; both are gated on the certified\n  Connector program.\nschemes:\n- id: oidc_externalgateway\n  type: openIdConnect\n  provider: Keycloak (WO Central)\n  realm: externalgateway\n  openIdConnectUrl: https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration\n  issuer: https://sso.wocentral.com/auth/realms/externalgateway\n  endpoints:\n    authorization: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/auth\n    token: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/token\n    jwks: https://sso.wocentral.com/auth/realms/externalgateway/protocol/openid-connect/certs\n  grant_types:\n  - authorization_code\n\
  \  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  observed_gateway_client: apigateway\n  observed_default_scope: openid\n  environments:\n    production: https://sso.wocentral.com/auth/realms/externalgateway\n    pre-production: https://ppe-sso.wocentral.com/auth/realms/externalgateway\n  applies_to: WideOrbit.io API Gateway (https://apigateway.wideorbit.com)\n- id: wo_data_api_header_keys\n  type: apiKey\n  in: header\n  applies_to: WO Data API (DAPI) 4.2.1\n  source: >-\n    \"WO Data API uses HTTP request header information to authorize requests and\n    authenticate users.\" — WO Data API Guide 4.2.1, Authentication\n  names:\n  - name: partner-id\n    required: true\n    description: Identifies the certified software provider calling the API.\n  - name: api-key\n \
  \   required: true\n    description: The secret issued to that partner.\n  - name: agreement-key\n    required: true\n    description: >-\n      Identifies the contractual data area. \"Each combination uniquely\n      identifies the area of WO Network, WO Traffic, or WO Omni data to be\n      accessed and the API client requesting access.\" This header is the tenancy\n      boundary.\n  model: closed\n  model_note: >-\n    \"DAPI uses the closed authentication model, where client authentication and\n    usage patterns are managed by WideOrbit.\" Credentials are provisioned by\n    WideOrbit Support; there is no registration endpoint, no token exchange, no\n    expiry and no rotation procedure documented.\n  failure:\n    status: 401\n    body: '{ \"Error\": \"Unauthorized access\" }'\n    note: >-\n      Returned when no valid combination is found. Authentication and\n      authorization failures are not distinguished.\n  callback_subset:\n    note: >-\n      The integrator's callback\
  \ acknowledgement POST to\n      {root}/api/Requests/Update/{requestId} carries only partner-id and api-key\n      — agreement-key is not required on that call.\n  transport: HTTPS (\"We do recommend, always use HTTPS secure endpoint.\")\n- id: wo_data_api_diagnostic_key\n  type: apiKey\n  in: header\n  applies_to: '{root}/api/Diagnostic/status_check'\n  names:\n  - name: DiagnosticSecurityKey\n    required: true\n    description: >-\n      A separate GUID-shaped key guarding the broadcaster connection health\n      check. Does not use the partner/api/agreement triple.\nnotes: >-\n  Access is limited to WideOrbit-certified partners; credentials are provisioned\n  through the WideOrbit.io program rather than self-service registration. No\n  HTTP-basic scheme was observed on either surface, and no mutual TLS is\n  required of callers (the Keycloak realm advertises tls_client_auth and\n  tls_client_certificate_bound_access_tokens as available client-authentication\n  options, but WideOrbit\
  \ does not document requiring them). The WO Data API's\n  header keys carry no environment prefix, so a client cannot tell a test\n  credential from a live one by inspection.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideorbit/refs/heads/main/authentication/wideorbit-authentication.yml
summary_line: 3 schemes
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
