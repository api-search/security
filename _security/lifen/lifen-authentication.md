---
api_key_in:
- header
api_specs:
- filename: lifen-fhir-api-openapi.json
  format: json
  label: Lifen FHIR API
  slug: lifen-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-fhir-api-openapi.json
- filename: lifen-authentication-api-openapi.json
  format: json
  label: Lifen Authentication API
  slug: lifen-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-authentication-api-openapi.json
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lifen Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Lifen secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Lifen
provider_slug: lifen
scheme_count: 3
schemes:
- applied_as: Authorization header, "Bearer {access_token}"
  flow: clientCredentials
  name: client_credentials
  notes: Machine-to-machine access to the FHIR API. `audience` selects the environment (https://production.platform-apis/ or https://post-prod.platform-apis/) and `database_reference` binds the token to one healthcare organisation. Credentials are issued by a Lifen account manager, not self-service.
  request_parameters:
  - client_id
  - client_secret
  - audience
  - database_reference
  - grant_type
  sources:
  - openapi/lifen-authentication-api-openapi.json
  - https://developer.lifen.fr/docs/machine-to-machine-communications
  token_endpoint: https://authentication.lifen.fr/v1/token
  token_endpoint_test: https://authentication.post-prod.lifen.fr/v1/token
  token_lifetime_seconds: 172800
  token_type: Bearer
  type: oauth2
- authorization_endpoint: https://authentication.lifen.fr/authorize
  code_challenge_methods:
  - S256
  flow: authorizationCode
  issuer: https://login.lifen.fr/
  jwks_uri: https://authentication.lifen.fr/.well-known/jwks.json
  logout_endpoint: https://api.lifen.fr/sso/v1/session/logout
  name: sso_oidc
  notes: User-facing SSO for embedding Lifen in a partner application; PKCE-only public client.
  pkce: true
  sources:
  - well-known/lifen-oauth-authorization-server.json
  - https://developer.lifen.fr/docs/sso-api
  token_endpoint: https://authentication.lifen.fr/v1/authorization_code/token
  token_endpoint_auth_methods:
  - none
  type: openIdConnect
- in: header
  name: sec0
  notes: How the published OpenAPI models the bearer token (x-bearer-format bearer). Functionally this is the OAuth 2.0 access token from the client_credentials scheme above, not a static API key.
  parameter: Authorization
  sources:
  - openapi/lifen-fhir-api-openapi.json
  type: apiKey
slug: lifen-authentication
source_filename: lifen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.lifen.fr/docs/machine-to-machine-communications\ndocs: https://developer.lifen.fr/docs/machine-to-machine-communications\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\nschemes:\n- name: client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://authentication.lifen.fr/v1/token\n  token_endpoint_test: https://authentication.post-prod.lifen.fr/v1/token\n  request_parameters:\n  - client_id\n  - client_secret\n  - audience\n  - database_reference\n  - grant_type\n  token_type: Bearer\n  token_lifetime_seconds: 172800\n  applied_as: Authorization header, \"Bearer {access_token}\"\n  notes: >-\n    Machine-to-machine access to the FHIR API. `audience` selects the environment\n    (https://production.platform-apis/ or https://post-prod.platform-apis/) and `database_reference`\n\
  \    binds the token to one healthcare organisation. Credentials are issued by a Lifen account\n    manager, not self-service.\n  sources:\n  - openapi/lifen-authentication-api-openapi.json\n  - https://developer.lifen.fr/docs/machine-to-machine-communications\n- name: sso_oidc\n  type: openIdConnect\n  flow: authorizationCode\n  issuer: https://login.lifen.fr/\n  authorization_endpoint: https://authentication.lifen.fr/authorize\n  token_endpoint: https://authentication.lifen.fr/v1/authorization_code/token\n  jwks_uri: https://authentication.lifen.fr/.well-known/jwks.json\n  pkce: true\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  logout_endpoint: https://api.lifen.fr/sso/v1/session/logout\n  notes: >-\n    User-facing SSO for embedding Lifen in a partner application; PKCE-only public client.\n  sources:\n  - well-known/lifen-oauth-authorization-server.json\n  - https://developer.lifen.fr/docs/sso-api\n- name: sec0\n  type: apiKey\n  in: header\n  parameter:\
  \ Authorization\n  notes: >-\n    How the published OpenAPI models the bearer token (x-bearer-format bearer). Functionally this is\n    the OAuth 2.0 access token from the client_credentials scheme above, not a static API key.\n  sources:\n  - openapi/lifen-fhir-api-openapi.json\nwebhook_authentication:\n  mechanism: HMAC-SHA256 signature\n  header: x-lifen-platform-signature\n  secret: generated per application in the developer portal\n  ip_allowlist:\n    test:\n    - 15.236.169.32\n    production:\n    - 15.236.169.164\n    - 35.180.249.12\n  docs: https://developer.lifen.fr/docs/secure-your-webhooks\nscopes: scopes/lifen-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/authentication/lifen-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Healthcare
- FHIR
- Interoperability
- Health Data
- Electronic Health Records
- Medical Documents
- Secure Messaging
- France
- HL7
---
