---
api_key_in: []
api_specs:
- filename: nhs-digital-booking-api-openapi.yml
  format: yaml
  label: NHS Digital Booking API
  slug: nhs-digital-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-booking-api-openapi.yml
- filename: nhs-digital-communication-api-openapi.yml
  format: yaml
  label: NHS Digital communication API
  slug: nhs-digital-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-communication-api-openapi.yml
- filename: nhs-digital-message-api-openapi.yml
  format: yaml
  label: NHS Digital Message API
  slug: nhs-digital-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-message-api-openapi.yml
- filename: nhs-digital-metadata-api-openapi.yml
  format: yaml
  label: NHS Digital Metadata API
  slug: nhs-digital-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-metadata-api-openapi.yml
- filename: nhs-digital-r4-api-openapi.yml
  format: yaml
  label: NHS Digital R4 API
  slug: nhs-digital-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-r4-api-openapi.yml
- filename: nhs-digital-referral-api-openapi.yml
  format: yaml
  label: NHS Digital Referral API
  slug: nhs-digital-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-referral-api-openapi.yml
- filename: nhs-digital-slots-api-openapi.yml
  format: yaml
  label: NHS Digital Slots API
  slug: nhs-digital-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-slots-api-openapi.yml
- filename: nhs-digital-stu3-api-openapi.yml
  format: yaml
  label: NHS Digital STU3 API
  slug: nhs-digital-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-stu3-api-openapi.yml
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
