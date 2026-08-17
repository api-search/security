---
api_key_in: []
api_specs:
- filename: health-gorilla-binary-api-openapi.yml
  format: yaml
  label: Health Gorilla Binary API
  slug: health-gorilla-binary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-binary-api-openapi.yml
- filename: health-gorilla-capabilitystatement-api-openapi.yml
  format: yaml
  label: Health Gorilla CapabilityStatement API
  slug: health-gorilla-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-capabilitystatement-api-openapi.yml
- filename: health-gorilla-coverage-api-openapi.yml
  format: yaml
  label: Health Gorilla Coverage API
  slug: health-gorilla-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-coverage-api-openapi.yml
- filename: health-gorilla-diagnosticreport-api-openapi.yml
  format: yaml
  label: Health Gorilla DiagnosticReport API
  slug: health-gorilla-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-diagnosticreport-api-openapi.yml
- filename: health-gorilla-documentreference-api-openapi.yml
  format: yaml
  label: Health Gorilla DocumentReference API
  slug: health-gorilla-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-documentreference-api-openapi.yml
- filename: health-gorilla-observation-api-openapi.yml
  format: yaml
  label: Health Gorilla Observation API
  slug: health-gorilla-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-observation-api-openapi.yml
- filename: health-gorilla-patient-api-openapi.yml
  format: yaml
  label: Health Gorilla Patient API
  slug: health-gorilla-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-patient-api-openapi.yml
- filename: health-gorilla-practitioner-api-openapi.yml
  format: yaml
  label: Health Gorilla Practitioner API
  slug: health-gorilla-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-practitioner-api-openapi.yml
- filename: health-gorilla-requestgroup-api-openapi.yml
  format: yaml
  label: Health Gorilla RequestGroup API
  slug: health-gorilla-requestgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-requestgroup-api-openapi.yml
- filename: health-gorilla-servicerequest-api-openapi.yml
  format: yaml
  label: Health Gorilla ServiceRequest API
  slug: health-gorilla-servicerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-servicerequest-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http
description: Health Gorilla authenticates every API call with an OAuth 2.0 bearer access token and implements the SMART App Launch profile on top of FHIR. The authorization server is www.healthgorilla.com; the resource server is api.healthgorilla.com. Both a SMART configuration and an OpenID Connect discovery document are served anonymously from the API host, so the full endpoint set, grant set and scope set are machine-discoverable without onboarding. Scopes are bound to the client at registration and cannot be self-expanded.
kind: authentication
layout: security
method: searched
name: Health Gorilla Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- jwtBearer
- clientCredentials
overview: Health Gorilla secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, jwtBearer, and clientCredentials flow(s).
provider_name: Health Gorilla
provider_slug: health-gorilla
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 bearer access token presented as `Authorization: Bearer <token>` on every request to a protected FHIR endpoint.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/health-gorilla-openapi.yml
  type: http
- description: SMART App Launch authorization declared by the live FHIR CapabilityStatement (restful-security-service code SMART-on-FHIR) and by the SMART configuration document served at api.healthgorilla.com/.well-known/smart-configuration.
  flows:
  - authorizationUrl: https://www.healthgorilla.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://www.healthgorilla.com/oauth/token
    refresh_token: issued
    required_params:
    - response_type=code
    - client_id
    - redirect_uri
    - client_secret
    tokenUrl: https://www.healthgorilla.com/oauth/token
  - authorizationUrl: https://www.healthgorilla.com/oauth/authorize
    flow: implicit
    note: Client must re-authorize when the access token expires.
    refresh_token: not issued
    required_params:
    - response_type=token
    - client_id
    - redirect_uri
  - assertion_audience: https://api.healthgorilla.com/oauth/token
    assertion_signing_alg: HS256
    flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    required_params:
    - assertion
    - client_id
    tokenUrl: https://www.healthgorilla.com/oauth/token
  - flow: clientCredentials
    note: Used for the system/*.* backend-services scope tier and for securing customer-operated webhook endpoints (Subscription channel OAuth extension).
    tokenUrl: https://www.healthgorilla.com/oauth/token
  name: SMARTonFHIR
  smart_capabilities:
  - launch-standalone
  - client-public
  - client-confidential-symmetric
  - permission-offline
  - permission-user
  - permission-system
  - permission-hg
  - sso-openid-connect
  sources:
  - well-known/health-gorilla-smart-configuration.json
  - fhir/health-gorilla-r4-capabilitystatement.json
  - https://developer.healthgorilla.com/reference/oauth-20-authentication
  type: oauth2
- claims_supported:
  - sub
  - aud
  - iss
  - fhirUser
  - name
  - given_name
  - family_name
  - birthdate
  - gender
  name: OpenIDConnect
  openIdConnectUrl: https://api.healthgorilla.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - fhirUser
  sources:
  - well-known/health-gorilla-openid-configuration.json
  type: openIdConnect
slug: health-gorilla-authentication
source_filename: health-gorilla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/health-gorilla-openapi.yml\ndocs: https://developer.healthgorilla.com/reference/oauth-20-authentication\ndescription: >-\n  Health Gorilla authenticates every API call with an OAuth 2.0 bearer access\n  token and implements the SMART App Launch profile on top of FHIR. The\n  authorization server is www.healthgorilla.com; the resource server is\n  api.healthgorilla.com. Both a SMART configuration and an OpenID Connect\n  discovery document are served anonymously from the API host, so the full\n  endpoint set, grant set and scope set are machine-discoverable without\n  onboarding. Scopes are bound to the client at registration and cannot be\n  self-expanded.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, refreshToken, jwtBearer, clientCredentials]\n  smart_on_fhir: true\n  openid_connect: true\n  dynamic_client_registration: true\n  transport: TLS 1.2\
  \ or higher required; plain HTTP rejected\nauthorization_server:\n  issuer: https://www.healthgorilla.com\n  authorization_endpoint: https://www.healthgorilla.com/oauth/authorize\n  token_endpoint: https://www.healthgorilla.com/oauth/token\n  registration_endpoint: https://www.healthgorilla.com/oauth/register\n  introspection_endpoint: https://www.healthgorilla.com/oauth/info\n  revocation_endpoint: https://www.healthgorilla.com/oauth/cancel\n  userinfo_endpoint: https://www.healthgorilla.com/oauth/userinfo\n  jwks_uri: https://www.healthgorilla.com/.well-known/jwks.json\n  token_endpoint_auth_methods: [none, client_secret_post, private_key_jwt]\n  id_token_signing_alg_values_supported: [RS256]\n  discovery:\n  - {path: /.well-known/smart-configuration, host: api.healthgorilla.com, status: 200, file: well-known/health-gorilla-smart-configuration.json}\n  - {path: /.well-known/openid-configuration, host: api.healthgorilla.com, status: 200, file: well-known/health-gorilla-openid-configuration.json}\n\
  schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    OAuth 2.0 bearer access token presented as `Authorization: Bearer <token>`\n    on every request to a protected FHIR endpoint.\n  sources: [openapi/health-gorilla-openapi.yml]\n- name: SMARTonFHIR\n  type: oauth2\n  description: >-\n    SMART App Launch authorization declared by the live FHIR CapabilityStatement\n    (restful-security-service code SMART-on-FHIR) and by the SMART configuration\n    document served at api.healthgorilla.com/.well-known/smart-configuration.\n  smart_capabilities:\n  - launch-standalone\n  - client-public\n  - client-confidential-symmetric\n  - permission-offline\n  - permission-user\n  - permission-system\n  - permission-hg\n  - sso-openid-connect\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.healthgorilla.com/oauth/authorize\n    tokenUrl: https://www.healthgorilla.com/oauth/token\n    refreshUrl: https://www.healthgorilla.com/oauth/token\n\
  \    required_params: [response_type=code, client_id, redirect_uri, client_secret]\n    refresh_token: issued\n  - flow: implicit\n    authorizationUrl: https://www.healthgorilla.com/oauth/authorize\n    required_params: [response_type=token, client_id, redirect_uri]\n    refresh_token: not issued\n    note: Client must re-authorize when the access token expires.\n  - flow: jwtBearer\n    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: https://www.healthgorilla.com/oauth/token\n    required_params: [assertion, client_id]\n    assertion_signing_alg: HS256\n    assertion_audience: https://api.healthgorilla.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://www.healthgorilla.com/oauth/token\n    note: >-\n      Used for the system/*.* backend-services scope tier and for securing\n      customer-operated webhook endpoints (Subscription channel OAuth extension).\n  sources:\n  - well-known/health-gorilla-smart-configuration.json\n  - fhir/health-gorilla-r4-capabilitystatement.json\n\
  \  - https://developer.healthgorilla.com/reference/oauth-20-authentication\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.healthgorilla.com/.well-known/openid-configuration\n  claims_supported: [sub, aud, iss, fhirUser, name, given_name, family_name, birthdate, gender]\n  scopes_supported: [openid, profile, fhirUser]\n  sources: [well-known/health-gorilla-openid-configuration.json]\ntoken:\n  type: Bearer\n  lifetime_field: expires_in\n  example_lifetime_seconds: 3600\n  refresh: >-\n    Refresh tokens are issued for selected grants (authorization code). A\n    refreshed token is bound to the originally granted scope; scope cannot be\n    expanded on refresh.\n  validation: GET /oauth/info?access_token=<token> returns client_name, client_id, expires_in, scope\n  revocation: GET /oauth/cancel?token=<token> returns 200 OK and also invalidates the paired refresh token\n  version_pinning:\n    parameter: hg_rest_api_version\n    response_field: hg_rest_api_version\n\
  \    error: unsupported_api_version (400)\n    note: A specific REST API version may be bound to the token at issuance.\nfailure_modes:\n- {condition: expired token, status: 401, error: expired_token}\n- {condition: invalid token, status: 401, error: invalid_token}\n- {condition: missing required scope, status: 403, error: insufficient_scope}\n- {condition: client authentication failed / unknown client_id, status: 400, error: invalid_client}\n- {condition: bad or expired code, refresh token or assertion, status: 400, error: invalid_grant}\n- {condition: unsupported grant, status: 400, error: unsupported_grant_type}\nrelated:\n- scopes/health-gorilla-scopes.yml\n- well-known/health-gorilla-well-known.yml\n- fhir/health-gorilla-fhir.yml\n- conventions/health-gorilla-conventions.yml\nx-evidence:\n- {url: 'https://api.healthgorilla.com/.well-known/smart-configuration', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://api.healthgorilla.com/.well-known/openid-configuration', http_status:\
  \ 200, fetched: '2026-08-14'}\n- {url: 'https://www.healthgorilla.com/.well-known/jwks.json', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://developer.healthgorilla.com/reference/oauth-20-authentication.md', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://developer.healthgorilla.com/docs/token-lifecycle.md', http_status: 200, fetched: '2026-08-14'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/authentication/health-gorilla-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
- TEFCA
- QHIN
- Health Information Exchange
- Lab Results
- Clinical Documents
- SMART on FHIR
- Patient Records
- HL7
---
