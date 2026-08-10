---
api_key_in:
- header
api_specs:
- filename: passivelogic-account-api-openapi.yml
  format: yaml
  label: PassiveLogic Account API
  slug: passivelogic-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-account-api-openapi.yml
- filename: passivelogic-api-api-openapi.yml
  format: yaml
  label: PassiveLogic API
  slug: passivelogic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-api-api-openapi.yml
- filename: passivelogic-app-api-openapi.yml
  format: yaml
  label: PassiveLogic App API
  slug: passivelogic-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-app-api-openapi.yml
- filename: passivelogic-auth-groups-api-openapi.yml
  format: yaml
  label: PassiveLogic Auth Groups API
  slug: passivelogic-auth-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-auth-groups-api-openapi.yml
- filename: passivelogic-authentication-api-openapi.yml
  format: yaml
  label: PassiveLogic Authentication API
  slug: passivelogic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-authentication-api-openapi.yml
- filename: passivelogic-bindings-api-openapi.yml
  format: yaml
  label: PassiveLogic Bindings API
  slug: passivelogic-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-bindings-api-openapi.yml
- filename: passivelogic-default-api-openapi.yml
  format: yaml
  label: PassiveLogic Default API
  slug: passivelogic-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-default-api-openapi.yml
- filename: passivelogic-export-api-openapi.yml
  format: yaml
  label: PassiveLogic Export API
  slug: passivelogic-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-export-api-openapi.yml
- filename: passivelogic-graphql-api-openapi.yml
  format: yaml
  label: PassiveLogic Graph QL API
  slug: passivelogic-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-graphql-api-openapi.yml
- filename: passivelogic-health-api-openapi.yml
  format: yaml
  label: PassiveLogic Health API
  slug: passivelogic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-health-api-openapi.yml
- filename: passivelogic-images-api-openapi.yml
  format: yaml
  label: PassiveLogic Images API
  slug: passivelogic-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-images-api-openapi.yml
- filename: passivelogic-organization-api-openapi.yml
  format: yaml
  label: PassiveLogic Organization API
  slug: passivelogic-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-organization-api-openapi.yml
- filename: passivelogic-passivelogic-device-api-openapi.yml
  format: yaml
  label: PassiveLogic PassiveLogic Device API
  slug: passivelogic-passivelogic-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-passivelogic-device-api-openapi.yml
- filename: passivelogic-quantum-sync-api-openapi.yml
  format: yaml
  label: PassiveLogic Quantum Sync API
  slug: passivelogic-quantum-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-quantum-sync-api-openapi.yml
- filename: passivelogic-site-api-openapi.yml
  format: yaml
  label: PassiveLogic Site API
  slug: passivelogic-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-site-api-openapi.yml
- filename: passivelogic-tunnel-api-openapi.yml
  format: yaml
  label: PassiveLogic Tunnel API
  slug: passivelogic-tunnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-tunnel-api-openapi.yml
- filename: passivelogic-utility-api-openapi.yml
  format: yaml
  label: PassiveLogic Utility API
  slug: passivelogic-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-utility-api-openapi.yml
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Passivelogic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: PassiveLogic secures its APIs with apiKey, http, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: PassiveLogic
provider_slug: passivelogic
scheme_count: 5
schemes:
- description: Authentication using an XSRF protected JWT
  in: header
  name: XSRF header
  parameter: X-PL-AUTH
  sources:
  - openapi/passivelogic-rest-api-openapi.yml
  type: apiKey
- description: Basic authentication used only at login. The Quantum documentation shows a GET with basic auth against /api/auth/login returning a JSON object with authorization and refresh tokens.
  name: Basic Auth - login
  scheme: basic
  sources:
  - openapi/passivelogic-rest-api-openapi.yml
  - https://quantumalliance.org/documentation/
  type: http
- description: Long-lived API key issued to a user by GET /api/auth/api-key/generate. Per the Quantum documentation an API key "acts with the same permissions as a JWT for the user who generated them" and is intended for command-line and scripting use. Keys are revoked with DELETE /api/auth/api-key.
  in: header
  name: PL API Key
  parameter: PL-API-KEY
  sources:
  - openapi/passivelogic-rest-api-openapi.yml
  - https://quantumalliance.org/documentation/
  type: apiKey
- deprecated: true
  description: DEPRECATED - PL API Key in Bearer header
  in: header
  name: DEPRECATED - PL API Key
  parameter: 'Authorization: PL-API-KEY'
  sources:
  - openapi/passivelogic-rest-api-openapi.yml
  type: apiKey
- description: Not declared in the OpenAPI, but the actual interactive login path. Every /app/login/* operation in the spec is documented as "Redirects to external authentication provider (Keycloak)", and the public GET /api/util/externalauthconfig endpoint returns the issuer, authorization endpoint and account-management URI for the login.passivelogic.com "prod" realm. Supports authorization_code (PKCE S256), client_credentials, device_code, refresh_token, token-exchange and CIBA; DPoP and mTLS-bound access tokens are advertised.
  name: Keycloak OpenID Connect
  openIdConnectUrl: https://login.passivelogic.com/realms/prod/.well-known/openid-configuration
  sources:
  - well-known/passivelogic-openid-configuration.json
  - https://passivelogic.com/api/util/externalauthconfig
  type: openIdConnect
slug: passivelogic-authentication
source_filename: passivelogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/passivelogic-rest-api-openapi.yml\ndocs: https://quantumalliance.org/documentation/\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - header\n  identity_provider: Keycloak (external), realm \"prod\"\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\nschemes:\n- name: XSRF header\n  type: apiKey\n  in: header\n  parameter: X-PL-AUTH\n  description: Authentication using an XSRF protected JWT\n  sources:\n  - openapi/passivelogic-rest-api-openapi.yml\n- name: Basic Auth - login\n  type: http\n  scheme: basic\n  description: >-\n    Basic authentication used only at login. The Quantum documentation shows a GET with basic auth against\n    /api/auth/login returning a JSON object with authorization and refresh tokens.\n  sources:\n  - openapi/passivelogic-rest-api-openapi.yml\n  - https://quantumalliance.org/documentation/\n- name: PL API Key\n  type: apiKey\n  in:\
  \ header\n  parameter: PL-API-KEY\n  description: >-\n    Long-lived API key issued to a user by GET /api/auth/api-key/generate. Per the Quantum documentation an API key\n    \"acts with the same permissions as a JWT for the user who generated them\" and is intended for command-line and\n    scripting use. Keys are revoked with DELETE /api/auth/api-key.\n  sources:\n  - openapi/passivelogic-rest-api-openapi.yml\n  - https://quantumalliance.org/documentation/\n- name: 'DEPRECATED - PL API Key'\n  type: apiKey\n  in: header\n  parameter: 'Authorization: PL-API-KEY'\n  description: DEPRECATED - PL API Key in Bearer header\n  deprecated: true\n  sources:\n  - openapi/passivelogic-rest-api-openapi.yml\n- name: Keycloak OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://login.passivelogic.com/realms/prod/.well-known/openid-configuration\n  description: >-\n    Not declared in the OpenAPI, but the actual interactive login path. Every /app/login/* operation in the spec is\n   \
  \ documented as \"Redirects to external authentication provider (Keycloak)\", and the public\n    GET /api/util/externalauthconfig endpoint returns the issuer, authorization endpoint and account-management URI\n    for the login.passivelogic.com \"prod\" realm. Supports authorization_code (PKCE S256), client_credentials,\n    device_code, refresh_token, token-exchange and CIBA; DPoP and mTLS-bound access tokens are advertised.\n  sources:\n  - well-known/passivelogic-openid-configuration.json\n  - https://passivelogic.com/api/util/externalauthconfig\ntoken_signing:\n  jwks_endpoint: https://passivelogic.com/api/auth/keys\n  note: >-\n    PassiveLogic publishes the public keys used to sign its own JSON Web Tokens at GET /api/auth/keys (anonymous,\n    ES384 over P-384). The Keycloak realm publishes a separate JWKS at\n    https://login.passivelogic.com/realms/prod/protocol/openid-connect/certs.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://passivelogic.com/api/doc\n\
  \    http_status: 200\n  - url: https://passivelogic.com/api/util/externalauthconfig\n    http_status: 200\n  - url: https://passivelogic.com/api/auth/keys\n    http_status: 200\n  - url: https://login.passivelogic.com/realms/prod/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/authentication/passivelogic-authentication.yml
summary_line: apiKey/http/openIdConnect · 5 schemes
tags:
- Company
- digital-twin
- building-automation
- hvac
- smart-buildings
- autonomous-systems
- graphql
- ontology
- iot
- edge-computing
- physical-ai
- energy
---
