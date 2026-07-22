---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Patientsknowbest Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Patients Know Best secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Patients Know Best
provider_slug: patientsknowbest
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer access tokens obtained via the SMART on FHIR authorization flow. Tokens are presented on FHIR resource requests to fhir.patientsknowbest.com.
  name: SMARTonFHIR
  scheme: bearer
  smart_on_fhir: true
  sources:
  - https://wiki.patientsknowbest.com/space/api
  type: oauth2
slug: patientsknowbest-authentication
source_filename: patientsknowbest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://wiki.patientsknowbest.com/space/api\ndocs: https://wiki.patientsknowbest.com/space/api\nnotes: >-\n  Patients Know Best exposes a HL7 FHIR API (see the published FHIR Conformance /\n  CapabilityStatement at https://fhir.patientsknowbest.com/metadata). FHIR access is\n  secured with OAuth 2.0 following the SMART on FHIR pattern that is standard for\n  patient/provider FHIR access. Exact scope strings, authorization/token endpoints\n  and grant types are documented in the developer wiki (client-rendered) and issued\n  to onboarded integration partners; they are not machine-harvestable from a public,\n  unauthenticated endpoint, so only the confirmed auth model is recorded here — no\n  scope values are invented.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  smart_on_fhir: true\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  scheme: bearer\n  description: >-\n    OAuth 2.0 bearer access tokens\
  \ obtained via the SMART on FHIR authorization\n    flow. Tokens are presented on FHIR resource requests to fhir.patientsknowbest.com.\n  smart_on_fhir: true\n  sources:\n  - https://wiki.patientsknowbest.com/space/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patientsknowbest/refs/heads/main/authentication/patientsknowbest-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Health Records
- FHIR
- Interoperability
- Patient Data
- NHS
- HL7
---
