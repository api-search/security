---
api_key_in: []
api_specs:
- filename: booking-and-referral-fhir-api.yaml
  format: yaml
  label: Booking and Referral - FHIR API
  slug: booking-and-referral-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/booking-and-referral-fhir-api.yaml
- filename: nhs-app-api.yaml
  format: yaml
  label: NHS App API
  slug: nhs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-app-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhs Digital Authentication
name_suffix: Authentication
oauth_flows: []
overview: NHS Digital secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NHS Digital
provider_slug: nhs-digital
scheme_count: 1
schemes:
- name: OAuth_Token
  scheme: bearer
  sources:
  - openapi/booking-and-referral-fhir-api.yaml
  - openapi/e-referrals-service-api.yaml
  type: http
slug: nhs-digital-authentication
source_filename: nhs-digital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/booking-and-referral-fhir-api.yaml, openapi/e-referrals-service-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth_Token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/booking-and-referral-fhir-api.yaml\n  - openapi/e-referrals-service-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/authentication/nhs-digital-authentication.yml
summary_line: http · 1 scheme
tags:
- NHS
- health
- FHIR
- UK
- patient demographics
- prescriptions
- referrals
- clinical data
- digital health
- government
---
