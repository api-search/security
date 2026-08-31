---
api_key_in:
- header
api_specs:
- filename: medadvisor-3rd-party-integration-api-openapi.yml
  format: yaml
  label: MedAdvisor 3rd-Party Integration API
  slug: medadvisor-3rd-party-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-3rd-party-integration-api-openapi.yml
- filename: medadvisor-account-api-openapi.yml
  format: yaml
  label: MedAdvisor Account API
  slug: medadvisor-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-account-api-openapi.yml
- filename: medadvisor-booking-api-openapi.yml
  format: yaml
  label: MedAdvisor Booking API
  slug: medadvisor-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-booking-api-openapi.yml
- filename: medadvisor-bookingservice-api-openapi.yml
  format: yaml
  label: MedAdvisor Booking Service API
  slug: medadvisor-bookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-bookingservice-api-openapi.yml
- filename: medadvisor-calendarsetting-api-openapi.yml
  format: yaml
  label: MedAdvisor Calendar Setting API
  slug: medadvisor-calendarsetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-calendarsetting-api-openapi.yml
- filename: medadvisor-clinic-api-openapi.yml
  format: yaml
  label: MedAdvisor Clinic API
  slug: medadvisor-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-clinic-api-openapi.yml
- filename: medadvisor-communication-api-openapi.yml
  format: yaml
  label: MedAdvisor Communication API
  slug: medadvisor-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-communication-api-openapi.yml
- filename: medadvisor-config-api-openapi.yml
  format: yaml
  label: MedAdvisor Config API
  slug: medadvisor-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-config-api-openapi.yml
- filename: medadvisor-headoffice-api-openapi.yml
  format: yaml
  label: MedAdvisor Head Office API
  slug: medadvisor-headoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-headoffice-api-openapi.yml
- filename: medadvisor-inbox-api-openapi.yml
  format: yaml
  label: MedAdvisor Inbox API
  slug: medadvisor-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-inbox-api-openapi.yml
- filename: medadvisor-logging-api-openapi.yml
  format: yaml
  label: MedAdvisor Logging API
  slug: medadvisor-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-logging-api-openapi.yml
- filename: medadvisor-pharmacist-api-openapi.yml
  format: yaml
  label: MedAdvisor Pharmacist API
  slug: medadvisor-pharmacist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacist-api-openapi.yml
- filename: medadvisor-pharmacy-api-openapi.yml
  format: yaml
  label: MedAdvisor Pharmacy API
  slug: medadvisor-pharmacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-api-openapi.yml
- filename: medadvisor-refillorder-api-openapi.yml
  format: yaml
  label: MedAdvisor Refill Order API
  slug: medadvisor-refillorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-refillorder-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Medadvisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: MedAdvisor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MedAdvisor
provider_slug: medadvisor
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  in: header
  name: Bearer
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/medadvisor-pharmacy-unified-openapi.json
  - openapi/medadvisor-pharmacy-unified-v2-openapi.json
  type: apiKey
slug: medadvisor-authentication
source_filename: medadvisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/medadvisor-pharmacy-unified-openapi.json\ndocs: https://pharmacy-unified.api.medadvisor.com.au/swagger/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: jwt-bearer\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme: bearer\n  bearer_format: JWT\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer {token}\"'\n  sources:\n  - openapi/medadvisor-pharmacy-unified-openapi.json\n  - openapi/medadvisor-pharmacy-unified-v2-openapi.json\ntoken_exchange:\n  operation: openapi/medadvisor-pharmacy-unified-openapi.json#Account_LoginPharmacy\n  endpoint: POST /api/v1/account/3rdpartylogin\n  description: >-\n    Integrators are issued a clientId and clientSecret by MedAdvisor. The pharmacy's\n    username and password are Base64-encoded (UTF-8) and posted with the clientId and\n    clientSecret to /3rdpartylogin; on success\
  \ the endpoint returns a JWT access token\n    used as Authorization: Bearer {token} on all subsequent requests.\n  onboarding: partner\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/authentication/medadvisor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Australia
- Pharmacy
- Medication Management
- Medication Adherence
- e-Prescribing
- eScript
- Patient Engagement
- Appointment Booking
- Digital Health
- Healthcare API
---
