---
api_key_in:
- header
api_specs:
- filename: dosespot-rest-api-jumpstart-epcs-v2-swagger.json
  format: json
  label: DoseSpot REST API - JumpStart + EPCS - V2
  slug: dosespot-rest-api-jumpstart-epcs-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/_original/dosespot-rest-api-jumpstart-epcs-v2-swagger.json
- filename: dosespot-rest-api-full-epcs-v2-swagger.json
  format: json
  label: DoseSpot REST API - Full + EPCS - V2
  slug: dosespot-rest-api-full-epcs-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/_original/dosespot-rest-api-full-epcs-v2-swagger.json
- filename: dosespot-medications-api-openapi.yml
  format: yaml
  label: DoseSpot Medications API
  slug: dosespot-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-medications-api-openapi.yml
- filename: dosespot-notifications-api-openapi.yml
  format: yaml
  label: DoseSpot Notifications API
  slug: dosespot-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-notifications-api-openapi.yml
- filename: dosespot-patients-api-openapi.yml
  format: yaml
  label: DoseSpot Patients API
  slug: dosespot-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-patients-api-openapi.yml
- filename: dosespot-pharmacies-api-openapi.yml
  format: yaml
  label: DoseSpot Pharmacies API
  slug: dosespot-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-pharmacies-api-openapi.yml
- filename: dosespot-prescribers-api-openapi.yml
  format: yaml
  label: DoseSpot Prescribers API
  slug: dosespot-prescribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-prescribers-api-openapi.yml
- filename: dosespot-prescriptions-api-openapi.yml
  format: yaml
  label: DoseSpot Prescriptions API
  slug: dosespot-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-prescriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dosespot Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoseSpot secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DoseSpot
provider_slug: dosespot
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth2 access token obtained from the DoseSpot token endpoint (POST /webapi/v2/connect/token) using your clinic and clinician credentials, sent as an Authorization: Bearer header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dosespot-medications-api-openapi.yml
  - openapi/dosespot-notifications-api-openapi.yml
  - openapi/dosespot-patients-api-openapi.yml
  - openapi/dosespot-pharmacies-api-openapi.yml
  - openapi/dosespot-prescribers-api-openapi.yml
  - openapi/dosespot-prescriptions-api-openapi.yml
  type: http
- description: Per-application subscription key issued by DoseSpot.
  in: header
  name: subscriptionKey
  parameter: Subscription-Key
  sources:
  - openapi/dosespot-medications-api-openapi.yml
  - openapi/dosespot-notifications-api-openapi.yml
  - openapi/dosespot-patients-api-openapi.yml
  - openapi/dosespot-pharmacies-api-openapi.yml
  - openapi/dosespot-prescribers-api-openapi.yml
  - openapi/dosespot-prescriptions-api-openapi.yml
  type: apiKey
slug: dosespot-authentication
source_filename: dosespot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: derived\nsource: openapi/dosespot-medications-api-openapi.yml, openapi/dosespot-notifications-api-openapi.yml,\n  openapi/dosespot-patients-api-openapi.yml, openapi/dosespot-pharmacies-api-openapi.yml, openapi/dosespot-prescribers-api-openapi.yml,\n  openapi/dosespot-prescriptions-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token obtained from the DoseSpot token endpoint (POST /webapi/v2/connect/token)\n    using your clinic and clinician credentials, sent as an Authorization: Bearer header.'\n  sources:\n  - openapi/dosespot-medications-api-openapi.yml\n  - openapi/dosespot-notifications-api-openapi.yml\n  - openapi/dosespot-patients-api-openapi.yml\n  - openapi/dosespot-pharmacies-api-openapi.yml\n  - openapi/dosespot-prescribers-api-openapi.yml\n  - openapi/dosespot-prescriptions-api-openapi.yml\n\
  - name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: Subscription-Key\n  description: Per-application subscription key issued by DoseSpot.\n  sources:\n  - openapi/dosespot-medications-api-openapi.yml\n  - openapi/dosespot-notifications-api-openapi.yml\n  - openapi/dosespot-patients-api-openapi.yml\n  - openapi/dosespot-pharmacies-api-openapi.yml\n  - openapi/dosespot-prescribers-api-openapi.yml\n  - openapi/dosespot-prescriptions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/authentication/dosespot-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- e-Prescribing
- eRx
- Healthcare
- EHR
- Pharmacy
- EPCS
- Prescriptions
- Clinical
- Medications
- Prior Authorization
- Surescripts
- Medi-Span
- Telehealth
- PDMP
- Digital Health
---
