---
api_key_in: []
api_specs:
- filename: hl7-fhir-r4-openapi.yml
  format: yaml
  label: HL7 FHIR R4 Healthcare API
  slug: hl7-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/openapi/hl7-fhir-r4-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hl7 Fhir Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HL7 FHIR secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HL7 FHIR
provider_slug: hl7-fhir
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://auth.example.com/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://auth.example.com/token
  name: SMARTonFHIR
  sources:
  - openapi/hl7-fhir-r4-openapi.yml
  type: oauth2
slug: hl7-fhir-authentication
source_filename: hl7-fhir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hl7-fhir-r4-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.example.com/authorize\n    tokenUrl: https://auth.example.com/token\n    scopes: 7\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/authentication/hl7-fhir-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Clinical
- FHIR
- Healthcare
- HL7
- Interoperability
---
