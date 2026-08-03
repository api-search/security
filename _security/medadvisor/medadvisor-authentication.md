---
api_key_in:
- header
api_specs:
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - 3rd-Party Integration
  slug: pharmacy-unified-third-party-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Booking Service
  slug: pharmacy-unified-booking-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Refill Order
  slug: pharmacy-unified-refill-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Inbox
  slug: pharmacy-unified-inbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Communication
  slug: pharmacy-unified-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Head Office
  slug: pharmacy-unified-head-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Pharmacy
  slug: pharmacy-unified-pharmacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-v2-openapi.json
  format: json
  label: MedAdvisor Pharmacy Unified API v2.0
  slug: medadvisor-pharmacy-unified-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-v2-openapi.json
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
