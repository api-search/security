---
api_key_in: []
api_specs:
- filename: nhs-england-booking-api-openapi.yml
  format: yaml
  label: NHS England Booking API
  slug: nhs-england-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-booking-api-openapi.yml
- filename: nhs-england-callbacks-api-openapi.yml
  format: yaml
  label: NHS England Callbacks API
  slug: nhs-england-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-callbacks-api-openapi.yml
- filename: nhs-england-channels-api-openapi.yml
  format: yaml
  label: NHS England Channels API
  slug: nhs-england-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-channels-api-openapi.yml
- filename: nhs-england-codesystem-api-openapi.yml
  format: yaml
  label: NHS England Code System API
  slug: nhs-england-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-codesystem-api-openapi.yml
- filename: nhs-england-communication-api-openapi.yml
  format: yaml
  label: NHS England Communication API
  slug: nhs-england-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-communication-api-openapi.yml
- filename: nhs-england-immunization-api-openapi.yml
  format: yaml
  label: NHS England Immunization API
  slug: nhs-england-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-immunization-api-openapi.yml
- filename: nhs-england-list-id-api-openapi.yml
  format: yaml
  label: NHS England List{id} API
  slug: nhs-england-list-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-list-id-api-openapi.yml
- filename: nhs-england-message-api-openapi.yml
  format: yaml
  label: NHS England Message API
  slug: nhs-england-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-message-api-openapi.yml
- filename: nhs-england-message-batches-api-openapi.yml
  format: yaml
  label: NHS England Message Batches API
  slug: nhs-england-message-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-message-batches-api-openapi.yml
- filename: nhs-england-messages-api-openapi.yml
  format: yaml
  label: NHS England Messages API
  slug: nhs-england-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-messages-api-openapi.yml
- filename: nhs-england-metadata-api-openapi.yml
  format: yaml
  label: NHS England Metadata API
  slug: nhs-england-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-metadata-api-openapi.yml
- filename: nhs-england-organisation-api-openapi.yml
  format: yaml
  label: NHS England Organisation API
  slug: nhs-england-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-organisation-api-openapi.yml
- filename: nhs-england-organization-api-openapi.yml
  format: yaml
  label: NHS England Organization API
  slug: nhs-england-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-organization-api-openapi.yml
- filename: nhs-england-organizationaffiliation-api-openapi.yml
  format: yaml
  label: NHS England Organization Affiliation API
  slug: nhs-england-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-organizationaffiliation-api-openapi.yml
- filename: nhs-england-r4-api-openapi.yml
  format: yaml
  label: NHS England R4 API
  slug: nhs-england-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-r4-api-openapi.yml
- filename: nhs-england-referral-api-openapi.yml
  format: yaml
  label: NHS England Referral API
  slug: nhs-england-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-referral-api-openapi.yml
- filename: nhs-england-slots-api-openapi.yml
  format: yaml
  label: NHS England Slots API
  slug: nhs-england-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-slots-api-openapi.yml
- filename: nhs-england-stu3-api-openapi.yml
  format: yaml
  label: NHS England STU3 API
  slug: nhs-england-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-stu3-api-openapi.yml
- filename: nhs-england-valueset-api-openapi.yml
  format: yaml
  label: NHS England Value Set API
  slug: nhs-england-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-england-valueset-api-openapi.yml
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
