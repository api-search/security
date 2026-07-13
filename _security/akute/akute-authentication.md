---
api_key_in:
- header
api_specs:
- filename: akute-openapi.yml
  format: yaml
  label: Akute Patients API
  slug: patients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Encounters API
  slug: encounters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Tasks API
  slug: tasks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Medications API
  slug: medications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Labs API
  slug: labs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
- filename: akute-openapi.yml
  format: yaml
  label: Akute Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Akute Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akute Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Akute Health
provider_slug: akute
scheme_count: 1
schemes:
- description: API key created on the Settings -> Developer page in Akute. Required on every request.
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/akute-openapi.yml
  type: apiKey
slug: akute-authentication
source_filename: akute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/akute-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key created on the Settings -> Developer page in Akute. Required on every\n    request.\n  sources:\n  - openapi/akute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/authentication/akute-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- EHR
- EMR
- FHIR
- Digital Health
- Telehealth
---
