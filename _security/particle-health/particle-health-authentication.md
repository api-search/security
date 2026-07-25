---
api_key_in: []
api_specs:
- filename: particle-health-authentication-api-openapi.yml
  format: yaml
  label: Particle Health Authentication API
  slug: particle-health-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-authentication-api-openapi.yml
- filename: particle-health-batches-api-openapi.yml
  format: yaml
  label: Particle Health Batches API
  slug: particle-health-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-batches-api-openapi.yml
- filename: particle-health-ccda-api-openapi.yml
  format: yaml
  label: Particle Health CCDA API
  slug: particle-health-ccda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-ccda-api-openapi.yml
- filename: particle-health-deltas-api-openapi.yml
  format: yaml
  label: Particle Health Deltas API
  slug: particle-health-deltas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-deltas-api-openapi.yml
- filename: particle-health-documents-api-openapi.yml
  format: yaml
  label: Particle Health Documents API
  slug: particle-health-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-documents-api-openapi.yml
- filename: particle-health-fhir-api-openapi.yml
  format: yaml
  label: Particle Health FHIR API
  slug: particle-health-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-fhir-api-openapi.yml
- filename: particle-health-files-api-openapi.yml
  format: yaml
  label: Particle Health Files API
  slug: particle-health-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-files-api-openapi.yml
- filename: particle-health-flat-api-openapi.yml
  format: yaml
  label: Particle Health Flat API
  slug: particle-health-flat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-flat-api-openapi.yml
- filename: particle-health-hl7v2-api-openapi.yml
  format: yaml
  label: Particle Health HL7v2 API
  slug: particle-health-hl7v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-hl7v2-api-openapi.yml
- filename: particle-health-networkparticipants-api-openapi.yml
  format: yaml
  label: Particle Health NetworkParticipants API
  slug: particle-health-networkparticipants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-networkparticipants-api-openapi.yml
- filename: particle-health-notifications-api-openapi.yml
  format: yaml
  label: Particle Health Notifications API
  slug: particle-health-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-notifications-api-openapi.yml
- filename: particle-health-patients-api-openapi.yml
  format: yaml
  label: Particle Health Patients API
  slug: particle-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-patients-api-openapi.yml
- filename: particle-health-projects-api-openapi.yml
  format: yaml
  label: Particle Health Projects API
  slug: particle-health-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-projects-api-openapi.yml
- filename: particle-health-providermap-api-openapi.yml
  format: yaml
  label: Particle Health ProviderMap API
  slug: particle-health-providermap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-providermap-api-openapi.yml
- filename: particle-health-queries-api-openapi.yml
  format: yaml
  label: Particle Health Queries API
  slug: particle-health-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-queries-api-openapi.yml
- filename: particle-health-signal-api-openapi.yml
  format: yaml
  label: Particle Health Signal API
  slug: particle-health-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-signal-api-openapi.yml
- filename: particle-health-subscriptions-api-openapi.yml
  format: yaml
  label: Particle Health Subscriptions API
  slug: particle-health-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-health/refs/heads/main/openapi/particle-health-subscriptions-api-openapi.yml
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
