---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: aerones-operations-hub-openapi.json
  format: json
  label: Aerones Operations Hub API
  slug: aerones-operations-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/openapi/aerones-operations-hub-openapi.json
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aerones Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- ciba
- refreshToken
overview: Aerones secures its APIs with apiKey, http, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, ciba, and refreshToken flow(s).
provider_name: Aerones
provider_slug: aerones
scheme_count: 4
schemes:
- applied_to_operations: 1086
  name: APIKeyAuth
  scheme: bearer
  sources:
  - openapi/aerones-operations-hub-openapi.json
  type: http
- applied_to_operations: 3
  name: AuthBearer
  note: A second bearer scheme, identical in shape to APIKeyAuth, applied to three operations.
  scheme: bearer
  sources:
  - openapi/aerones-operations-hub-openapi.json
  type: http
- applied_to_operations: 1086
  in: cookie
  name: CookieAuth
  note: Django session cookie - the browser path used by portal.aerones.com.
  parameter: opshub_prod_sessionid
  sources:
  - openapi/aerones-operations-hub-openapi.json
  type: apiKey
- authorization_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth
  backchannel_authentication_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/ext/ciba/auth
  client_id_observed: operations-hub
  device_authorization_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth/device
  end_session_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/logout
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token/introspect
  issuer: https://sso.aerones.com/realms/aerones
  jwks_uri: https://sso.aerones.com/realms/aerones/protocol/openid-connect/certs
  name: KeycloakOIDC
  openIdConnectUrl: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration
  pkce_methods:
  - plain
  - S256
  registration_endpoint: https://sso.aerones.com/realms/aerones/clients-registrations/openid-connect
  revocation_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/revoke
  sources:
  - well-known/aerones-sso-aerones-openid-configuration.json
  token_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
  userinfo_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/userinfo
slug: aerones-authentication
source_filename: aerones-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/aerones-operations-hub-openapi.json\ndocs: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration\nnote: >-\n  Derived from the published OpenAPI securitySchemes, then upgraded with the Keycloak\n  OIDC discovery document probed on sso.aerones.com. 1,089 of 1,114 operations declare\n  security; the 25 that do not are the auth endpoints themselves plus the schema and\n  the inbound webhook receivers. The OpenAPI declares no oauth2 scheme - the bearer\n  token it accepts is issued by the Keycloak realm below, so the OIDC layer is not\n  visible in the spec and has to be read off the discovery document.\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - ciba\n  - refreshToken\nschemes:\n- name: APIKeyAuth\n  type: http\n  scheme: bearer\n  applied_to_operations: 1086\n  sources:\n  -\
  \ openapi/aerones-operations-hub-openapi.json\n- name: AuthBearer\n  type: http\n  scheme: bearer\n  applied_to_operations: 3\n  note: A second bearer scheme, identical in shape to APIKeyAuth, applied to three operations.\n  sources:\n  - openapi/aerones-operations-hub-openapi.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: opshub_prod_sessionid\n  applied_to_operations: 1086\n  note: Django session cookie - the browser path used by portal.aerones.com.\n  sources:\n  - openapi/aerones-operations-hub-openapi.json\n- name: KeycloakOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration\n  issuer: https://sso.aerones.com/realms/aerones\n  authorization_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth\n  token_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token\n  userinfo_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/userinfo\n\
  \  jwks_uri: https://sso.aerones.com/realms/aerones/protocol/openid-connect/certs\n  introspection_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/revoke\n  end_session_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/logout\n  device_authorization_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth/device\n  registration_endpoint: https://sso.aerones.com/realms/aerones/clients-registrations/openid-connect\n  backchannel_authentication_endpoint: https://sso.aerones.com/realms/aerones/protocol/openid-connect/ext/ciba/auth\n  client_id_observed: operations-hub\n  pkce_methods:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n\
  \  - password\n  - client_credentials\n  - urn:openid:params:grant-type:ciba\n  - urn:ietf:params:oauth:grant-type:device_code\n  sources:\n  - well-known/aerones-sso-aerones-openid-configuration.json\nx-evidence:\n- url: https://operations.aerones.com/api/openapi.json\n  http_status: 200\n  fetched: '2026-09-10'\n- url: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-09-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/authentication/aerones-authentication.yml
summary_line: apiKey/http/openIdConnect · 4 schemes
tags:
- Company
- Wind Energy
- Renewable Energy
- Robotics
- Drones
- Inspection
- Field Service Management
- Asset Management
- Industrial
- Energy
- Maintenance
- Latvia
---
