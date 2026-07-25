---
api_key_in: []
api_specs:
- filename: nhs-e-referral-service-openapi.yaml
  format: yaml
  label: e-Referral Service (e-RS) - FHIR API
  slug: nhs-e-referral-service-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-e-referral-service-openapi.yaml
- filename: nhs-booking-and-referral-fhir-openapi.yaml
  format: yaml
  label: Booking and Referral Standard (BaRS) - FHIR API
  slug: nhs-booking-and-referral-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-booking-and-referral-fhir-openapi.yaml
- filename: nhs-immunisation-history-openapi.yaml
  format: yaml
  label: Immunisation History - FHIR API
  slug: nhs-immunisation-history-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-immunisation-history-openapi.yaml
- filename: nhs-organisation-data-service-fhir-r4-openapi.yaml
  format: yaml
  label: Organisation Data Service (ODS) - FHIR API
  slug: nhs-organisation-data-service-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-organisation-data-service-fhir-r4-openapi.yaml
- filename: nhs-app-openapi.yaml
  format: yaml
  label: NHS App API
  slug: nhs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-app-openapi.yaml
- filename: nhs-communications-manager-openapi.yaml
  format: yaml
  label: NHS Notify (Communications Manager) API
  slug: nhs-notify-communications-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-communications-manager-openapi.yaml
- filename: nhs-service-search-openapi.yaml
  format: yaml
  label: Service Search (Directory of Healthcare Services) API
  slug: nhs-service-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-service-search-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhs England Authentication
name_suffix: Authentication
oauth_flows: []
overview: NHS England secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NHS England
provider_slug: nhs-england
scheme_count: 1
schemes:
- name: OAuth_Token
  scheme: bearer
  sources:
  - openapi/nhs-booking-and-referral-fhir-openapi.yaml
  - openapi/nhs-e-referral-service-openapi.yaml
  type: http
slug: nhs-england-authentication
source_filename: nhs-england-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/nhs-booking-and-referral-fhir-openapi.yaml, openapi/nhs-e-referral-service-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth_Token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nhs-booking-and-referral-fhir-openapi.yaml\n  - openapi/nhs-e-referral-service-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/authentication/nhs-england-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- United Kingdom
- National Health System
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Health Data
- e-Prescribing
- EHR
---
