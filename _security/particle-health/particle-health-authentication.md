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
method: searched
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
  service_account:
    creation: Reach out to a Particle Health representative, or self-serve via the Management API (Create Service Account + Create Credentials endpoints).
    scope_format: projects/<project_id>
    token_ttl_seconds: 3600
  sources:
  - openapi/particle-health-authentication-api-openapi.yml
  - openapi/particle-health-batches-api-openapi.yml
  - openapi/particle-health-ccda-api-openapi.yml
  - openapi/particle-health-deltas-api-openapi.yml
  - openapi/particle-health-documents-api-openapi.yml
  - openapi/particle-health-fhir-api-openapi.yml
  - openapi/particle-health-files-api-openapi.yml
  - openapi/particle-health-flat-api-openapi.yml
  - openapi/particle-health-hl7v2-api-openapi.yml
  - openapi/particle-health-networkparticipants-api-openapi.yml
  - openapi/particle-health-notifications-api-openapi.yml
  - openapi/particle-health-patients-api-openapi.yml
  - openapi/particle-health-projects-api-openapi.yml
  - openapi/particle-health-providermap-api-openapi.yml
  - openapi/particle-health-queries-api-openapi.yml
  - openapi/particle-health-signal-api-openapi.yml
  - openapi/particle-health-subscriptions-api-openapi.yml
  type: http
slug: particle-health-authentication
source_filename: particle-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\ndocs:\n  - https://docs.particlehealth.com/docs/auth-and-keys\n  - https://raw.githubusercontent.com/ParticleHealth/particle-connect/main/agent-documentation/08-authentication.md\nsource: openapi/particle-health-authentication-api-openapi.yml, openapi/particle-health-batches-api-openapi.yml,\n  openapi/particle-health-ccda-api-openapi.yml, openapi/particle-health-deltas-api-openapi.yml,\n  openapi/particle-health-documents-api-openapi.yml, openapi/particle-health-fhir-api-openapi.yml,\n  openapi/particle-health-files-api-openapi.yml, openapi/particle-health-flat-api-openapi.yml,\n  openapi/particle-health-hl7v2-api-openapi.yml, openapi/particle-health-networkparticipants-api-openapi.yml,\n  openapi/particle-health-notifications-api-openapi.yml, openapi/particle-health-patients-api-openapi.yml,\n  openapi/particle-health-projects-api-openapi.yml, openapi/particle-health-providermap-api-openapi.yml,\n  openapi/particle-health-queries-api-openapi.yml,\
  \ openapi/particle-health-signal-api-openapi.yml,\n  openapi/particle-health-subscriptions-api-openapi.yml\nsummary:\n  types:\n  - http\nnotes: >-\n  Particle documents the flow as \"OAuth 2 Client-Credentials,\" but the actual request is a\n  provider-specific GET (not the standard OAuth 2 token POST): GET https://sandbox.particlehealth.com/auth\n  (or the production host) with client-id, client-secret, and scope sent as request HEADERS, returning\n  a plain-text JWT (not a JSON token response). scope is formatted projects/<project_id> and selects the\n  project the token is bound to. Tokens are valid for 1 hour. A second, separate credential pair (org-level,\n  not project-level) is used for the Management API auth flow, which is instead a POST to the same /auth\n  path and can return either JSON or URL-encoded form data. Source for the GET/headers/plain-text-JWT\n  behavior is Particle Health's own public GitHub quickstart (ParticleHealth/particle-connect), which\n  documents both\
  \ flows in implementation detail (file:line pointers into their SDK source); this\n  supplements, and does not contradict, the docs.particlehealth.com auth page.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2 client-credentials JWT issued by `/auth`. Token expires after one hour.\n  sources:\n  - openapi/particle-health-authentication-api-openapi.yml\n  - openapi/particle-health-batches-api-openapi.yml\n  - openapi/particle-health-ccda-api-openapi.yml\n  - openapi/particle-health-deltas-api-openapi.yml\n  - openapi/particle-health-documents-api-openapi.yml\n  - openapi/particle-health-fhir-api-openapi.yml\n  - openapi/particle-health-files-api-openapi.yml\n  - openapi/particle-health-flat-api-openapi.yml\n  - openapi/particle-health-hl7v2-api-openapi.yml\n  - openapi/particle-health-networkparticipants-api-openapi.yml\n  - openapi/particle-health-notifications-api-openapi.yml\n  - openapi/particle-health-patients-api-openapi.yml\n\
  \  - openapi/particle-health-projects-api-openapi.yml\n  - openapi/particle-health-providermap-api-openapi.yml\n  - openapi/particle-health-queries-api-openapi.yml\n  - openapi/particle-health-signal-api-openapi.yml\n  - openapi/particle-health-subscriptions-api-openapi.yml\n  service_account:\n    creation: Reach out to a Particle Health representative, or self-serve via the Management API\n      (Create Service Account + Create Credentials endpoints).\n    token_ttl_seconds: 3600\n    scope_format: projects/<project_id>\n"
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
