---
api_key_in:
- header
api_specs:
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Patients API
  slug: dosespot-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescriptions API
  slug: dosespot-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Medications API
  slug: dosespot-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Pharmacies API
  slug: dosespot-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescribers API
  slug: dosespot-prescribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Notifications API
  slug: dosespot-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
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
  - openapi/dosespot-openapi.yml
  type: http
- description: Per-application subscription key issued by DoseSpot.
  in: header
  name: subscriptionKey
  parameter: Subscription-Key
  sources:
  - openapi/dosespot-openapi.yml
  type: apiKey
slug: dosespot-authentication
source_filename: dosespot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dosespot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token obtained from the DoseSpot token endpoint (POST /webapi/v2/connect/token)\n    using your clinic and clinician credentials, sent as an Authorization: Bearer header.'\n  sources:\n  - openapi/dosespot-openapi.yml\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: Subscription-Key\n  description: Per-application subscription key issued by DoseSpot.\n  sources:\n  - openapi/dosespot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/authentication/dosespot-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- e-Prescribing
- eRx
- Healthcare
- EHR
- Pharmacy
- EPCS
---
