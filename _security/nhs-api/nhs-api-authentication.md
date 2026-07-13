---
api_key_in: []
api_specs:
- filename: personal-demographics-service-api
  format: yaml
  label: Personal Demographics Service - FHIR API
  slug: personal-demographics-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/personal-demographics-service-api
- filename: gp-connect-access-record-fhir-api
  format: yaml
  label: GP Connect Access Record Structured - FHIR API
  slug: gp-connect-access-record-structured-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/gp-connect-access-record-fhir-api
- filename: gp-connect-appointments-management-fhir
  format: yaml
  label: GP Connect Appointment Management - FHIR API
  slug: gp-connect-appointment-management-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/gp-connect-appointments-management-fhir
- filename: electronic-prescription-service-api
  format: yaml
  label: Electronic Prescription Service - FHIR API
  slug: electronic-prescription-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/electronic-prescription-service-api
- filename: openapi.yaml
  format: yaml
  label: NHS Login API
  slug: nhs-login-api
  spec_type: OpenAPI
  url: https://nhsconnect.github.io/nhslogin/scopes-and-claims/
- filename: organisation-data-service-fhir-api
  format: yaml
  label: Organisation Data Service - FHIR API
  slug: organisation-data-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/organisation-data-service-fhir-api
- filename: spine-directory-service-api
  format: yaml
  label: Spine Directory Service - FHIR API
  slug: spine-directory-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/spine-directory-service-api
- filename: e-referrals-service-api
  format: yaml
  label: NHS e-Referral Service - FHIR API
  slug: nhs-e-referral-service-fhir-api
  spec_type: OpenAPI
  url: https://github.com/NHSDigital/e-referrals-service-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhs Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: NHS API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NHS API
provider_slug: nhs-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/e-referrals-service-api.yaml
  type: http
slug: nhs-api-authentication
source_filename: nhs-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/e-referrals-service-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/e-referrals-service-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/authentication/nhs-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- FHIR
- NHS
- UK
- HL7
- Electronic Prescriptions
- Patient Demographics
- GP Connect
- NHS Login
- Interoperability
---
