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
name: Eclinicalworks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: eClinicalWorks secures its APIs with oauth2, openIdConnect, and http across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: eClinicalWorks
provider_slug: eclinicalworks
scheme_count: 7
schemes:
- authorizationUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/authorize
  client_auth:
  - client_secret_basic (symmetric)
  - private_key_jwt (asymmetric, RS384)
  description: SMART on FHIR EHR Launch. App launches from inside an eClinicalWorks EHR session and receives launch context (patient, encounter, banner, style).
  flow: authorizationCode
  name: smart-on-fhir-ehr-launch
  sources:
  - well-known/eclinicalworks-smart-configuration.json
  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/provider/ehr-launch-asymmetric
  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token
  type: oauth2
- authorizationUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/authorize
  client_auth:
  - client_secret_basic (symmetric)
  - private_key_jwt (asymmetric, RS384)
  description: SMART on FHIR Standalone Launch. App launches outside the EHR; launch/patient requests patient selection at authorization time.
  flow: authorizationCode
  name: smart-on-fhir-standalone-launch
  sources:
  - well-known/eclinicalworks-smart-configuration.json
  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/provider/standalone-symmetric
  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token
  type: oauth2
- client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
  description: SMART Backend Services (system-to-system, no user). App registers a JWKS URL on the eCW Dev Portal, mints a one-time client_assertion JWT signed RS384, and exchanges it at the token endpoint for a system/* scoped bearer token. Used for single-patient backend access and Group/$export bulk data.
  flow: clientCredentials
  jwks: Registered by the developer on the eCW Dev Portal; must be reachable and allow-listed by eClinicalWorks.
  name: smart-backend-services
  notes: system/Group.read must be included in every bulk (Group) token request and must NOT be included for the Backend Single Patient API.
  signing_alg: RS384
  sources:
  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/backend/authentication
  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token
  type: oauth2
- description: SSO via OpenID Connect; sso-openid-connect is advertised in the SMART capabilities. openid + fhirUser (or openid + profile) identify the logged-in user.
  jwks_uri: https://oauthserver.eclinicalworks.com/oauth/oauth2/jwks
  name: openid-connect
  sources:
  - well-known/eclinicalworks-smart-configuration.json
  type: openIdConnect
- description: RFC 7662 style token introspection per SMART App Launch STU2. HTTP POST with application/x-www-form-urlencoded; confidential clients authenticate with HTTP Basic (base64 client_id:client_secret). Response carries active, scope, client_id, exp.
  name: token-introspection
  sources:
  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/token-introspection
  type: oauth2-introspection
- description: Separate authorization surface for the healow RPM Vendor (Tracker) API. Asymmetric client credentials issued per app by the healow Dev Portal; client_assertion signed RS384; tokens are scoped system/Observation.create system/Device.create.
  flow: clientCredentials
  name: healow-tracker-backend-services
  sources:
  - https://connect4.healow.com/apps/jsp/dev/r4/fhirRpmVendorDocumentation.jsp
  tokenUrl: https://connect4.healow.com/apps/api/v1/fhir/tracker/oauth/token
  type: oauth2
- description: 'Outbound calls healow makes to an RPM vendor are authenticated with X-Client-Id plus X-Server-Signature: Base64(HMAC_SHA256(<request-body>, <vendor-client-secret>)). For DELETE the signature is computed over an empty body.'
  name: healow-tracker-callback-signing
  scheme: hmac
  sources:
  - https://connect4.healow.com/apps/jsp/dev/r4/fhirRpmVendorDocumentation.jsp
  type: http
slug: eclinicalworks-authentication
source_filename: eclinicalworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://fhir4.eclinicalworks.com/fhir/r4/FEIGCD/.well-known/smart-configuration\ndocs: https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started\nnote: eClinicalWorks publishes no OpenAPI. The authentication profile below is read from the live SMART\n  on FHIR configuration document and the FHIR CapabilityStatement served by the eCW FHIR Facade, plus\n  the eClinicalWorks Platform for Open Development and healow developer-portal authentication pages. Both\n  the provider-facing (fhir4.eclinicalworks.com) and patient-facing healow (fhir4.healow.com) facades\n  share one authorization server at oauthserver.eclinicalworks.com.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  client_authentication:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_jwt\n  pkce: S256 (required for public\
  \ clients)\n  asymmetric_signing_alg: RS384 only (private_key_jwt / Backend Services)\n  api_key_in: []\n  mutual_tls: false\nschemes:\n- name: smart-on-fhir-ehr-launch\n  type: oauth2\n  flow: authorizationCode\n  description: SMART on FHIR EHR Launch. App launches from inside an eClinicalWorks EHR session and receives\n    launch context (patient, encounter, banner, style).\n  authorizationUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/authorize\n  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token\n  client_auth:\n  - client_secret_basic (symmetric)\n  - private_key_jwt (asymmetric, RS384)\n  sources:\n  - well-known/eclinicalworks-smart-configuration.json\n  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/provider/ehr-launch-asymmetric\n- name: smart-on-fhir-standalone-launch\n  type: oauth2\n  flow: authorizationCode\n  description: SMART on FHIR Standalone Launch. App launches outside the EHR; launch/patient requests\n    patient\
  \ selection at authorization time.\n  authorizationUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/authorize\n  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token\n  client_auth:\n  - client_secret_basic (symmetric)\n  - private_key_jwt (asymmetric, RS384)\n  sources:\n  - well-known/eclinicalworks-smart-configuration.json\n  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/provider/standalone-symmetric\n- name: smart-backend-services\n  type: oauth2\n  flow: clientCredentials\n  description: SMART Backend Services (system-to-system, no user). App registers a JWKS URL on the eCW\n    Dev Portal, mints a one-time client_assertion JWT signed RS384, and exchanges it at the token endpoint\n    for a system/* scoped bearer token. Used for single-patient backend access and Group/$export bulk\n    data.\n  tokenUrl: https://oauthserver.eclinicalworks.com/oauth/oauth2/token\n  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n\
  \  signing_alg: RS384\n  jwks: Registered by the developer on the eCW Dev Portal; must be reachable and allow-listed by eClinicalWorks.\n  notes: system/Group.read must be included in every bulk (Group) token request and must NOT be included\n    for the Backend Single Patient API.\n  sources:\n  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/backend/authentication\n- name: openid-connect\n  type: openIdConnect\n  description: SSO via OpenID Connect; sso-openid-connect is advertised in the SMART capabilities. openid\n    + fhirUser (or openid + profile) identify the logged-in user.\n  jwks_uri: https://oauthserver.eclinicalworks.com/oauth/oauth2/jwks\n  sources:\n  - well-known/eclinicalworks-smart-configuration.json\n- name: token-introspection\n  type: oauth2-introspection\n  description: RFC 7662 style token introspection per SMART App Launch STU2. HTTP POST with application/x-www-form-urlencoded;\n    confidential clients authenticate with HTTP Basic (base64\
  \ client_id:client_secret). Response carries\n    active, scope, client_id, exp.\n  sources:\n  - https://fhir.eclinicalworks.com/ecwopendev/documentation/getting-started/token-introspection\n- name: healow-tracker-backend-services\n  type: oauth2\n  flow: clientCredentials\n  description: Separate authorization surface for the healow RPM Vendor (Tracker) API. Asymmetric client\n    credentials issued per app by the healow Dev Portal; client_assertion signed RS384; tokens are scoped\n    system/Observation.create system/Device.create.\n  tokenUrl: https://connect4.healow.com/apps/api/v1/fhir/tracker/oauth/token\n  sources:\n  - https://connect4.healow.com/apps/jsp/dev/r4/fhirRpmVendorDocumentation.jsp\n- name: healow-tracker-callback-signing\n  type: http\n  scheme: hmac\n  description: 'Outbound calls healow makes to an RPM vendor are authenticated with X-Client-Id plus X-Server-Signature:\n    Base64(HMAC_SHA256(<request-body>, <vendor-client-secret>)). For DELETE the signature is computed\n\
  \    over an empty body.'\n  sources:\n  - https://connect4.healow.com/apps/jsp/dev/r4/fhirRpmVendorDocumentation.jsp\nbearer_token:\n  header: 'Authorization: Bearer <access_token>'\n  token_type: Bearer\n  access_token_lifetime_seconds_example: 300\n  note: 'Documented token response example shows expires_in: 300 for the eCW Backend Services flow and\n    expires_in: 30000 for the healow Tracker flow.'\nscopes_artifact: scopes/eclinicalworks-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclinicalworks/refs/heads/main/authentication/eclinicalworks-authentication.yml
summary_line: oauth2/openIdConnect/http · 7 schemes
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Practice Management
- Clinical Data
- Health Information Exchange
- Patient Data
- Appointments
- Billing
- SMART on FHIR
- US Core
- USCDI
- Bulk Data
- Remote Patient Monitoring
- Interoperability
- ONC Certified
- CDS Hooks
- healow
---
