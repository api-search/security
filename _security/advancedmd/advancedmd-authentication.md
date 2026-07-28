---
api_key_in:
- header
api_specs:
- filename: advancedmd-fhir-single-api-openapi.json
  format: json
  label: AdvancedMD FHIR Single API (US Core 6.1.0)
  slug: advancedmd-fhir-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-single-api-openapi.json
- filename: advancedmd-fhir-bulk-api-openapi.json
  format: json
  label: AdvancedMD FHIR Bulk API
  slug: advancedmd-fhir-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-bulk-api-openapi.json
- filename: advancedmd-application-access-apis-swagger.json
  format: json
  label: AdvancedMD Application Access APIs (Legacy Patient APIs)
  slug: advancedmd-application-access-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-application-access-apis-swagger.json
auth_types:
- oauth2
- openIdConnect
- apiKey
- http
description: 'The specs are thin — every FHIR document declares only a bare `bearerAuth` (http/bearer/JWT) scheme and says nothing about how that JWT is obtained. The real model is SMART-on-FHIR OAuth 2.0: three-legged authorization_code (with PKCE) for patient and practitioner apps, and SMART Backend Services client_credentials with an RS384 private_key_jwt assertion for Bulk Data. The legacy Application Access APIs use a separate api-key + session-token model.'
kind: authentication
layout: security
method: searched
name: Advancedmd Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: AdvancedMD secures its APIs with oauth2, openIdConnect, apiKey, and http across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: AdvancedMD
provider_slug: advancedmd
scheme_count: 7
schemes:
- applies_to:
  - advancedmd:advancedmd-fhir-single-api
  authorizationUrl: https://providerapi.advancedmd.com/v1/oauth2/authorize
  authorization_code_lifetime: about one minute
  client_authentication:
  - client_secret_basic
  - private_key_jwt
  context_returned:
  - patient
  - fhirUser
  - userId
  - aud
  - scope
  - need_patient_banner
  - smart_style_url
  flow: authorizationCode
  name: SMART-on-FHIR OAuth 2.0 (three-legged)
  note: Used for patient- and provider-facing apps. Both standalone launch and EHR launch are supported (capabilities launch-standalone, launch-ehr, context-ehr-patient, context-ehr-encounter, authorize-post).
  pkce: S256
  refresh_token_lifetime_seconds: 7775999
  sources:
  - fhir/advancedmd-smart-configuration.json
  - https://fhir.advancedmd.com/fhir/launch-and-authorization
  tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token
  token_lifetime_seconds: 3599
  type: oauth2
- additional_parameters:
  - username
  - password
  - officekey
  applies_to:
  - advancedmd:advancedmd-fhir-bulk-api
  assertion:
    body_claims:
    - iss
    - sub
    - aud
    - exp
    - jti
    client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
    header_claims:
    - alg
    - kid
    - typ
    - jku
    one_time_use: true
    signing_alg: RS384
  client_authentication: private_key_jwt
  flow: clientCredentials
  name: SMART Backend Services (two-legged, Bulk only)
  note: AdvancedMD states it does "not support two-legged OAuth for system-to-system interactions" generally — this flow exists only for FHIR Bulk Data Access.
  scope: system/*.read
  sources:
  - https://fhir.advancedmd.com/fhir/launch-and-authorization
  tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token
  token_lifetime: one hour
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS384
  - RS256
  issuer: https://providerapi.advancedmd.com/v1/r4
  name: OpenID Connect
  openIdConnectUrl: https://providerapi.advancedmd.com/v1/r4/.well-known/openid-configuration
  scopes:
  - openid
  - fhirUser
  sources:
  - fhir/advancedmd-openid-configuration.json
  type: openIdConnect
- bearerFormat: JWT
  name: bearerAuth
  note: How the specs model the SMART access token. It is the transport, not the grant.
  scheme: bearer
  sources:
  - openapi/advancedmd-fhir-bulk-api-openapi.json
  - openapi/advancedmd-fhir-single-api-openapi.json
  type: http
- applies_to:
  - advancedmd:advancedmd-application-access-apis
  in: header
  name: API Key
  parameter: apikey
  sources:
  - openapi/advancedmd-application-access-apis-swagger.json
  type: apiKey
- applies_to:
  - advancedmd:advancedmd-application-access-apis
  in: header
  name: Bearer Token
  note: Session token minted by POST /authenticate from a Patient Portal username, password and practice office key. Modelled as an apiKey rather than http/bearer in the Swagger.
  parameter: Authorization
  sources:
  - openapi/advancedmd-application-access-apis-swagger.json
  type: apiKey
- applies_to:
  - advancedmd:advancedmd-fhir-bulk-jwks-api
  name: HTTP Basic (Bulk JWKS helper)
  note: Bulk application Key as username and Secret as password, for the test-only POST /v1/fhir-jwks/token endpoint.
  scheme: basic
  sources:
  - https://fhir.advancedmd.com/fhir/bulk-api
  type: http
slug: advancedmd-authentication
source_filename: advancedmd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Derived from the securityDefinitions/securitySchemes in\n  openapi/advancedmd-application-access-apis-swagger.json,\n  openapi/advancedmd-fhir-bulk-api-openapi.json and\n  openapi/advancedmd-fhir-single-api-openapi.json, then upgraded from the provider's own\n  documentation: https://fhir.advancedmd.com/fhir/launch-and-authorization,\n  https://fhir.advancedmd.com/getting-started, https://fhir.advancedmd.com/fhir/bulk-api,\n  and the live discovery documents at /v1/r4/.well-known/smart-configuration and\n  /v1/r4/.well-known/openid-configuration.\ndocs: https://fhir.advancedmd.com/fhir/launch-and-authorization\ndescription: >-\n  The specs are thin — every FHIR document declares only a bare `bearerAuth` (http/bearer/JWT)\n  scheme and says nothing about how that JWT is obtained. The real model is SMART-on-FHIR\n  OAuth 2.0: three-legged authorization_code (with PKCE) for patient and practitioner apps,\n  and SMART Backend\
  \ Services client_credentials with an RS384 private_key_jwt assertion for\n  Bulk Data. The legacy Application Access APIs use a separate api-key + session-token model.\nsummary:\n  types: [oauth2, openIdConnect, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  mtls: false\n  two_legged_oauth_for_general_access: false\nschemes:\n  - name: SMART-on-FHIR OAuth 2.0 (three-legged)\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://providerapi.advancedmd.com/v1/oauth2/authorize\n    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token\n    pkce: S256\n    client_authentication: [client_secret_basic, private_key_jwt]\n    token_lifetime_seconds: 3599\n    refresh_token_lifetime_seconds: 7775999\n    authorization_code_lifetime: about one minute\n    context_returned: [patient, fhirUser, userId, aud, scope, need_patient_banner, smart_style_url]\n    applies_to:\n      - advancedmd:advancedmd-fhir-single-api\n \
  \   sources:\n      - fhir/advancedmd-smart-configuration.json\n      - https://fhir.advancedmd.com/fhir/launch-and-authorization\n    note: >-\n      Used for patient- and provider-facing apps. Both standalone launch and EHR launch are\n      supported (capabilities launch-standalone, launch-ehr, context-ehr-patient,\n      context-ehr-encounter, authorize-post).\n  - name: SMART Backend Services (two-legged, Bulk only)\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token\n    client_authentication: private_key_jwt\n    assertion:\n      client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n      signing_alg: RS384\n      header_claims: [alg, kid, typ, jku]\n      body_claims: [iss, sub, aud, exp, jti]\n      one_time_use: true\n    additional_parameters: [username, password, officekey]\n    scope: system/*.read\n    token_lifetime: one hour\n    applies_to:\n      - advancedmd:advancedmd-fhir-bulk-api\n\
  \    sources:\n      - https://fhir.advancedmd.com/fhir/launch-and-authorization\n    note: >-\n      AdvancedMD states it does \"not support two-legged OAuth for system-to-system\n      interactions\" generally — this flow exists only for FHIR Bulk Data Access.\n  - name: OpenID Connect\n    type: openIdConnect\n    openIdConnectUrl: https://providerapi.advancedmd.com/v1/r4/.well-known/openid-configuration\n    issuer: https://providerapi.advancedmd.com/v1/r4\n    id_token_signing_alg_values_supported: [RS384, RS256]\n    scopes: [openid, fhirUser]\n    sources:\n      - fhir/advancedmd-openid-configuration.json\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - openapi/advancedmd-fhir-bulk-api-openapi.json\n      - openapi/advancedmd-fhir-single-api-openapi.json\n    note: How the specs model the SMART access token. It is the transport, not the grant.\n  - name: API Key\n    type: apiKey\n    in: header\n    parameter: apikey\n   \
  \ applies_to:\n      - advancedmd:advancedmd-application-access-apis\n    sources:\n      - openapi/advancedmd-application-access-apis-swagger.json\n  - name: Bearer Token\n    type: apiKey\n    in: header\n    parameter: Authorization\n    applies_to:\n      - advancedmd:advancedmd-application-access-apis\n    sources:\n      - openapi/advancedmd-application-access-apis-swagger.json\n    note: >-\n      Session token minted by POST /authenticate from a Patient Portal username, password\n      and practice office key. Modelled as an apiKey rather than http/bearer in the Swagger.\n  - name: HTTP Basic (Bulk JWKS helper)\n    type: http\n    scheme: basic\n    applies_to:\n      - advancedmd:advancedmd-fhir-bulk-jwks-api\n    sources:\n      - https://fhir.advancedmd.com/fhir/bulk-api\n    note: Bulk application Key as username and Secret as password, for the test-only POST /v1/fhir-jwks/token endpoint.\nendpoints:\n  authorization: https://providerapi.advancedmd.com/v1/oauth2/authorize\n\
  \  token: https://providerapi.advancedmd.com/v1/oauth2/token\n  introspection: https://providerapi.advancedmd.com/v1/oauth2/introspect\n  revocation: https://providerapi.advancedmd.com/v1/oauth2/revoke\n  management: https://providerapi.advancedmd.com/v1/oauth2/manage\n  jwks: https://providerapi.advancedmd.com/v1/oauth2/.well-known/jwks.json\n  smart_configuration: https://providerapi.advancedmd.com/v1/r4/.well-known/smart-configuration\n  openid_configuration: https://providerapi.advancedmd.com/v1/r4/.well-known/openid-configuration\nonboarding:\n  registration: Self-service developer + app registration at https://fhir.advancedmd.com\n  approval: >-\n    Manual — email InterOps@advancedmd.com with subject \"FHIR App Approval Request for\n    Appname: [Your Appname]\" and your redirect URL. \"It can take a few days.\"\n  constraint: One product per application — a Single-patient app must not also request the Bulk or non-FHIR products.\n  credentials: The app's Key is the client_id and\
  \ its Secret is the client_secret.\n  cost: Free for the certified FHIR APIs (Developer Terms of Service, last updated 2022-11-28).\nscopes: scopes/advancedmd-scopes.yml\ngated_surfaces:\n  - name: Connect APIs (REST + XML-RPC) and ODBC driver\n    auth: Not publicly documented — credentials issued under a signed Certified API Developer Agreement with licensing and support fees.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/authentication/advancedmd-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/http · 7 schemes
tags:
- Healthcare
- United States
- EHR
- EMR
- Practice Management
- Medical Billing
- FHIR
- HL7
- SMART on FHIR
- US Core
- Interoperability
- Revenue Cycle Management
- Scheduling
---
