---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aidbox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
- token-exchange
overview: Aidbox secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, clientCredentials, and token-exchange flow(s).
provider_name: Aidbox
provider_slug: aidbox
scheme_count: 3
schemes:
- authorizationUrl: https://sandbox.aidbox.app/auth/authorize
  client_types:
  - client-confidential-symmetric
  - client-confidential-asymmetric
  - client-public
  grant_types:
  - authorization_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - implicit
  - password
  - client_credentials
  introspectionUrl: https://sandbox.aidbox.app/auth/introspect
  jwksUri: https://sandbox.aidbox.app/.well-known/jwks.json
  launch_contexts:
  - launch-ehr
  - launch-standalone
  - context-ehr-patient
  - context-ehr-encounter
  - context-standalone-patient
  name: SMART-on-FHIR / OAuth2
  note: SMART App Launch (EHR launch + standalone launch), SMART Backend Services via client_credentials + private_key_jwt (asymmetric), and OIDC single-sign-on.
  pkce:
  - S256
  tokenUrl: https://sandbox.aidbox.app/auth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
  userinfoUrl: https://sandbox.aidbox.app/auth/userinfo
- claims:
  - sub
  - aud
  - email
  - exp
  - iat
  - iss
  - locale
  - family_name
  - given_name
  - name
  - picture
  id_token_signing_alg:
  - RS256
  name: OpenID Connect
  openIdConnectUrl: https://sandbox.aidbox.app/.well-known/openid-configuration
  type: openIdConnect
- name: Basic
  note: HTTP Basic authentication is advertised in the CapabilityStatement security service list, typically for Client resources / trusted server-to-server access.
  scheme: basic
  type: http
slug: aidbox-authentication
source_filename: aidbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  well-known/aidbox-smart-configuration.json, well-known/aidbox-openid-configuration.json,\n  well-known/aidbox-oauth-authorization-server.json, fhir/aidbox-capabilitystatement.json,\n  https://www.health-samurai.io/docs/aidbox/modules/security-and-access-control\ndocs: https://www.health-samurai.io/docs/aidbox/modules/security-and-access-control\nsummary:\n  types: [oauth2, openIdConnect, http]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode, implicit, password, clientCredentials, token-exchange]\n  smart_on_fhir: true\n  api_key_in: []\nschemes:\n- name: SMART-on-FHIR / OAuth2\n  type: oauth2\n  authorizationUrl: https://sandbox.aidbox.app/auth/authorize\n  tokenUrl: https://sandbox.aidbox.app/auth/token\n  introspectionUrl: https://sandbox.aidbox.app/auth/introspect\n  userinfoUrl: https://sandbox.aidbox.app/auth/userinfo\n  jwksUri: https://sandbox.aidbox.app/.well-known/jwks.json\n  grant_types:\
  \ [authorization_code, urn:ietf:params:oauth:grant-type:token-exchange, implicit, password, client_credentials]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n  pkce: [S256]\n  launch_contexts: [launch-ehr, launch-standalone, context-ehr-patient, context-ehr-encounter, context-standalone-patient]\n  client_types: [client-confidential-symmetric, client-confidential-asymmetric, client-public]\n  note: >-\n    SMART App Launch (EHR launch + standalone launch), SMART Backend Services via\n    client_credentials + private_key_jwt (asymmetric), and OIDC single-sign-on.\n- name: OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://sandbox.aidbox.app/.well-known/openid-configuration\n  id_token_signing_alg: [RS256]\n  claims: [sub, aud, email, exp, iat, iss, locale, family_name, given_name, name, picture]\n- name: Basic\n  type: http\n  scheme: basic\n  note: >-\n    HTTP Basic authentication is advertised in the CapabilityStatement security\
  \ service\n    list, typically for Client resources / trusted server-to-server access.\naccess_control:\n  models: [AccessPolicy, RBAC, SMART scopes (v1 + v2), label-based / relationship-based, SCIM]\n  note: >-\n    Aidbox layers its own AccessPolicy engine (JSON/SQL/Matcho/allow) over SMART scopes;\n    supports permission-v1 and permission-v2 SMART scope syntaxes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidbox/refs/heads/main/authentication/aidbox-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- EHR
- Health Data
- FHIR Server
- Bulk Data
- Terminology
- Digital Health
---
