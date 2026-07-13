---
api_key_in: []
api_specs:
- filename: charmhealth-fhir-api-openapi.yml
  format: yaml
  label: CharmHealth FHIR API
  slug: fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-fhir-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Charmhealth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: CharmHealth secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: CharmHealth
provider_slug: charmhealth
scheme_count: 1
schemes:
- description: SMART on FHIR authorization with patient/, user/, and system/ scopes.
  flows:
  - authorizationUrl: https://ehr2.charmtracker.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token
  name: smartOnFhir
  sources:
  - openapi/charmhealth-fhir-api-openapi.yml
  type: oauth2
slug: charmhealth-authentication
source_filename: charmhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charmhealth-fhir-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ehr2.charmtracker.com/oauth/v2/auth\n    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token\n    scopes: 6\n  - flow: clientCredentials\n    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token\n    scopes: 1\n  description: SMART on FHIR authorization with patient/, user/, and system/ scopes.\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/authentication/charmhealth-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
---
