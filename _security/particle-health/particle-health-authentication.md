---
api_key_in: []
api_specs:
- filename: particle-health-openapi.yml
  format: yaml
  label: Particle Health API
  slug: patient-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Particle Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Particle Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Particle Health
provider_slug: particle-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2 client-credentials JWT issued by `/auth`. Token expires after one hour.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/particle-health-openapi.yml
  type: http
slug: particle-health-authentication
source_filename: particle-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/particle-health-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2 client-credentials JWT issued by `/auth`. Token expires after one hour.\n  sources:\n  - openapi/particle-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/authentication/particle-health-authentication.yml
summary_line: http · 1 scheme
tags:
- ADT
- C-CDA
- Care Coordination
- Carequality
- Clinical Data
- CommonWell
- Deltas
- eHealth Exchange
- EHR
- FHIR
- Health Data
- Health Information Exchange
- Healthcare
- HIE
- HL7
- HL7v2
- Interoperability
- Medical Records
- Patients
- Pharmacy
- QHIN
- Surescripts
- TEFCA
- USCDI
---
