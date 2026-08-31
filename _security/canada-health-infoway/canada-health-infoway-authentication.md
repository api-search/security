---
api_key_in:
- query
- header
api_specs:
- filename: canada-health-infoway-capabilitystatement-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Capability Statement API
  slug: canada-health-infoway-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-capabilitystatement-api-openapi.yml
- filename: canada-health-infoway-codesystem-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Code System API
  slug: canada-health-infoway-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-codesystem-api-openapi.yml
- filename: canada-health-infoway-codesystems-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Codesystems API
  slug: canada-health-infoway-codesystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-codesystems-api-openapi.yml
- filename: canada-health-infoway-conceptmap-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Concept Map API
  slug: canada-health-infoway-conceptmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-conceptmap-api-openapi.yml
- filename: canada-health-infoway-maps-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Maps API
  slug: canada-health-infoway-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-maps-api-openapi.yml
- filename: canada-health-infoway-notification-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Notification API
  slug: canada-health-infoway-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-notification-api-openapi.yml
- filename: canada-health-infoway-packages-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Packages API
  slug: canada-health-infoway-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-packages-api-openapi.yml
- filename: canada-health-infoway-resourcelocations-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Resourcelocations API
  slug: canada-health-infoway-resourcelocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-resourcelocations-api-openapi.yml
- filename: canada-health-infoway-session-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Session API
  slug: canada-health-infoway-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-session-api-openapi.yml
- filename: canada-health-infoway-subsets-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Subsets API
  slug: canada-health-infoway-subsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-subsets-api-openapi.yml
- filename: canada-health-infoway-valueset-api-openapi.yml
  format: yaml
  label: Canada Health Infoway Value Set API
  slug: canada-health-infoway-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/openapi/canada-health-infoway-valueset-api-openapi.yml
auth_types:
- apiKey
- http
- session
description: ''
kind: authentication
layout: security
method: searched
name: Canada Health Infoway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canada Health Infoway secures its APIs with apiKey, http, and session across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canada Health Infoway
provider_slug: canada-health-infoway
scheme_count: 3
schemes:
- credential: username:password Base64-encoded
  in:
  - query
  - header
  name: basic-auth-credentials
  passed_as:
  - 'query parameter: auth (Base64 username:password)'
  - 'HTTP header: Authorization: Basic <base64>'
  scheme: basic
  sources:
  - openapi/infoway-fhir-terminology-service-api-openapi.json
  - openapi/infoway-terminology-service-api-openapi.json
  type: http
- description: JSON Web Token issued by the session login. Returned as 'btoken' from POST /rest/v1/session and accepted as a bearer/query token on subsequent reads.
  format: JWT
  in: query
  name: btoken-jwt
  parameter: btoken
  scheme: bearer
  sources:
  - openapi/infoway-terminology-service-api-openapi.json
  type: apiKey
- description: Single sign-on token (returned as 'authToken' from session login) for the Infoway SSO at auth-users.infoway-inforoute.ca.
  in: query
  name: ssotoken
  parameter: ssotoken
  sources:
  - openapi/infoway-terminology-service-api-openapi.json
  type: apiKey
slug: canada-health-infoway-authentication
source_filename: canada-health-infoway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/*-openapi.json parameter descriptions + Accelero developer docs\ndocs: https://accelero.infoway-inforoute.ca/en/tools/developer-tools/terminology-service-api\nsummary:\n  types: [apiKey, http, session]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  note: >-\n    Canada Health Infoway's Terminology Gateway does not declare OpenAPI securitySchemes\n    (both Swagger 2.0 specs omit securityDefinitions). Authentication is documented inline\n    on nearly every operation and via the RESTful session endpoint. Terminology CONTENT\n    reads are gated behind free account registration + an authenticated session; the FHIR\n    CapabilityStatement (/fhir/v1/metadata) is served anonymously. No OAuth2 / SMART-on-FHIR\n    scopes are used (no /.well-known/smart-configuration is served).\nschemes:\n- name: basic-auth-credentials\n  type: http\n  scheme: basic\n  in: [query, header]\n  credential: username:password Base64-encoded\n\
  \  passed_as:\n  - \"query parameter: auth (Base64 username:password)\"\n  - \"HTTP header: Authorization: Basic <base64>\"\n  sources: [openapi/infoway-fhir-terminology-service-api-openapi.json, openapi/infoway-terminology-service-api-openapi.json]\n- name: btoken-jwt\n  type: apiKey\n  in: query\n  parameter: btoken\n  scheme: bearer\n  format: JWT\n  description: >-\n    JSON Web Token issued by the session login. Returned as 'btoken' from POST /rest/v1/session\n    and accepted as a bearer/query token on subsequent reads.\n  sources: [openapi/infoway-terminology-service-api-openapi.json]\n- name: ssotoken\n  type: apiKey\n  in: query\n  parameter: ssotoken\n  description: >-\n    Single sign-on token (returned as 'authToken' from session login) for the Infoway SSO\n    at auth-users.infoway-inforoute.ca.\n  sources: [openapi/infoway-terminology-service-api-openapi.json]\nsession:\n  login: POST /rest/v1/session\n  logout: DELETE /rest/v1/session\n  accepts: [auth, btoken, ssotoken]\n\
  \  returns: [authToken (SSO token), btoken (JWT), profile attributes]\n  operationId: login\nregistration:\n  url: https://accelero.infoway-inforoute.ca/en/register\n  login_ui: https://auth-users.infoway-inforoute.ca/auth/UI/Login\n  cost: free\nanonymous_surface:\n- /fhir/v1/metadata (FHIR CapabilityStatement)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-health-infoway/refs/heads/main/authentication/canada-health-infoway-authentication.yml
summary_line: apiKey/http/session · 3 schemes
tags:
- Healthcare
- Canada
- FHIR
- HL7
- Interoperability
- Terminology
- National Health System
- Digital Health
- Standards
- CA Core
---
