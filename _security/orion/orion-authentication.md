---
api_key_in:
- header
api_specs:
- filename: orion-fhir-openapi.yml
  format: yaml
  label: Orion Health FHIR API
  slug: orion-health-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-fhir-openapi.yml
- filename: orion-population-health-openapi.yml
  format: yaml
  label: Orion Health Population Health API
  slug: orion-health-population-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-population-health-openapi.yml
- filename: orion-hie-openapi.yml
  format: yaml
  label: Orion Health HIE API
  slug: orion-health-hie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-hie-openapi.yml
- filename: orion-rhapsody-openapi.yml
  format: yaml
  label: Orion Health Rhapsody Integration API
  slug: orion-health-rhapsody-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-rhapsody-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Orion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Orion Health secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Orion Health
provider_slug: orion
scheme_count: 4
schemes:
- description: OAuth 2.0 authorization using SMART on FHIR
  flows:
  - authorizationUrl: https://auth.orionhealth.com/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  sources:
  - openapi/orion-fhir-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/orion-fhir-openapi.yml
  - openapi/orion-hie-openapi.yml
  - openapi/orion-population-health-openapi.yml
  - openapi/orion-rhapsody-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  sources:
  - openapi/orion-hie-openapi.yml
  - openapi/orion-population-health-openapi.yml
  - openapi/orion-rhapsody-openapi.yml
  type: oauth2
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/orion-rhapsody-openapi.yml
  type: apiKey
slug: orion-authentication
source_filename: orion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orion-fhir-openapi.yml, openapi/orion-hie-openapi.yml, openapi/orion-population-health-openapi.yml,\n  openapi/orion-rhapsody-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.orionhealth.com/oauth2/authorize\n    tokenUrl: https://auth.orionhealth.com/oauth2/token\n    scopes: 9\n  description: OAuth 2.0 authorization using SMART on FHIR\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/orion-fhir-openapi.yml\n  - openapi/orion-hie-openapi.yml\n  - openapi/orion-population-health-openapi.yml\n  - openapi/orion-rhapsody-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.orionhealth.com/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/orion-hie-openapi.yml\n  - openapi/orion-population-health-openapi.yml\n  - openapi/orion-rhapsody-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/orion-rhapsody-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/authentication/orion-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- EHR
- FHIR
- Health IT
- Healthcare
- HIE
- HL7
- Integration
- Interoperability
- Population Health
---
