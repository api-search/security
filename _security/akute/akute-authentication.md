---
api_key_in:
- header
api_specs:
- filename: akute-appointments-api-openapi.yml
  format: yaml
  label: Akute Health Appointments API
  slug: akute-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-appointments-api-openapi.yml
- filename: akute-documents-api-openapi.yml
  format: yaml
  label: Akute Health Documents API
  slug: akute-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-documents-api-openapi.yml
- filename: akute-encounters-api-openapi.yml
  format: yaml
  label: Akute Health Encounters API
  slug: akute-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-encounters-api-openapi.yml
- filename: akute-labs-api-openapi.yml
  format: yaml
  label: Akute Health Labs API
  slug: akute-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-labs-api-openapi.yml
- filename: akute-medications-api-openapi.yml
  format: yaml
  label: Akute Health Medications API
  slug: akute-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-medications-api-openapi.yml
- filename: akute-patients-api-openapi.yml
  format: yaml
  label: Akute Health Patients API
  slug: akute-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-patients-api-openapi.yml
- filename: akute-tasks-api-openapi.yml
  format: yaml
  label: Akute Health Tasks API
  slug: akute-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-tasks-api-openapi.yml
- filename: akute-webhooks-api-openapi.yml
  format: yaml
  label: Akute Health Webhooks API
  slug: akute-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-webhooks-api-openapi.yml
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
