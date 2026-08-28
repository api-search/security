---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Micro Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Micro Connect declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Micro Connect
provider_slug: micro-connect
scheme_count: 2
schemes:
- format: Bearer <access_token>
  in: header
  name: openIdConnect
  note: The Open Platform SPA obtains a Keycloak access token and presents it as a bearer token to the ShenYu gateway at https://api.mcisaas.com/api.
  openIdConnectUrl: https://kc.mcisaas.com/auth/realms/numa-realm/.well-known/openid-configuration
  parameter: Authorization
  type: openIdConnect
- authorization_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/auth
  device_authorization_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/auth/device
  end_session_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/logout
  flows:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  introspection_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/token/introspect
  jwks_uri: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/certs
  name: oauth2
  pushed_authorization_request_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/ext/par/request
  registration_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/clients-registrations/openid-connect
  revocation_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/revoke
  token_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/token
  type: oauth2
  userinfo_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/userinfo
slug: micro-connect-authentication
source_filename: micro-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://kc.mcisaas.com/auth/realms/numa-realm/.well-known/openid-configuration (HTTP 200)\n  and https://kc.mcisaas.com/auth/realms/master/.well-known/openid-configuration (HTTP 200),\n  saved verbatim in well-known/. Client identity read from Micro Connect's own published JS\n  (https://mcisaas.com/mcc-share/domain.js and the Open Platform bundle at\n  https://open.microconnect.cn/mcc-open/assets/index.4743a4fd.js).\ndocs: null\ndocs_note: >-\n  Micro Connect publishes no authentication documentation. Everything here was read off the\n  live, anonymous OpenID Connect discovery documents and the provider's own browser bundle;\n  nothing is inferred.\nsummary: >-\n  The Micro Connect SaaS estate authenticates against a self-hosted Keycloak identity\n  provider at kc.mcisaas.com using OpenID Connect / OAuth 2.0. There is no API-key surface,\n  no public client registration, and no published developer credential flow — an\
  \ integrator\n  must first be registered as an enterprise account on the Open Platform.\nidentity_provider:\n  product: Keycloak (self-hosted)\n  host: kc.mcisaas.com\n  path_style: legacy /auth/ prefix\n  realms:\n  - name: numa-realm\n    issuer: https://kc.mcisaas.com/auth/realms/numa-realm\n    used_by: >-\n      Micro Connect Open Platform SPA (open.microconnect.com / open.microconnect.cn),\n      clientId web-mcc-open-platform\n    discovery: https://kc.mcisaas.com/auth/realms/numa-realm/.well-known/openid-configuration\n    status: 200\n  - name: master\n    issuer: https://kc.mcisaas.com/auth/realms/master\n    used_by: Keycloak administration realm\n    discovery: https://kc.mcisaas.com/auth/realms/master/.well-known/openid-configuration\n    status: 200\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://kc.mcisaas.com/auth/realms/numa-realm/.well-known/openid-configuration\n  in: header\n  parameter: Authorization\n  format: Bearer <access_token>\n\
  \  note: >-\n    The Open Platform SPA obtains a Keycloak access token and presents it as a bearer token\n    to the ShenYu gateway at https://api.mcisaas.com/api.\n- name: oauth2\n  type: oauth2\n  flows:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  authorization_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/auth\n  token_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/token\n  introspection_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/token/introspect\n  userinfo_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/userinfo\n  revocation_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/revoke\n  end_session_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/logout\n\
  \  jwks_uri: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/certs\n  registration_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/clients-registrations/openid-connect\n  pushed_authorization_request_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/ext/par/request\n  device_authorization_endpoint: https://kc.mcisaas.com/auth/realms/numa-realm/protocol/openid-connect/auth/device\ncapabilities:\n  pkce: true\n  pkce_methods:\n  - plain\n  - S256\n  par_supported: true\n  par_required: false\n  mtls_bound_access_tokens: true\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  backchannel_logout: true\n  frontchannel_logout: true\n  dynamic_client_registration_endpoint_present: true\n  request_object_supported: true\nobservations:\n- >-\n  Strong protocol capability, zero developer-facing exposure: the identity provider supports\n  PKCE\
  \ (S256), Pushed Authorization Requests, mTLS-bound access tokens, private_key_jwt and\n  CIBA — a FAPI-grade toolkit — but none of it is documented anywhere a prospective\n  integrator can read, and no client can be obtained without an enrolled enterprise account.\n- >-\n  The `implicit` and `password` grants are still advertised as supported on both realms.\n  Both are discouraged by OAuth 2.0 Security Best Current Practice (RFC 9700) and removed in\n  OAuth 2.1; this is a Keycloak default rather than an explicit Micro Connect decision, but\n  it is what the discovery document advertises today.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro-connect/refs/heads/main/authentication/micro-connect-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Financial Services
- Capital Markets
- Exchanges
- Revenue Based Financing
- Fintech
- Investing
- Small Business
- Hong Kong
- Macao
- China
---
