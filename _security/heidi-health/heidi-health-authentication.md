---
api_key_in:
- header
api_specs:
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Authentication API
  slug: heidi-api-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Templates API
  slug: heidi-api-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Patient Profiles API
  slug: heidi-api-patient-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Sessions API
  slug: heidi-api-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Context API
  slug: heidi-api-session-context
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Coding API
  slug: heidi-api-session-coding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Transcription API
  slug: heidi-api-transcription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Consult Notes API
  slug: heidi-api-consult-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Documents API
  slug: heidi-api-documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Ask Heidi API
  slug: heidi-api-ask-heidi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Heidi Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heidi Health secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Heidi Health
provider_slug: heidi-health
scheme_count: 2
schemes:
- in: header
  name: heidiApiKey
  parameter: Heidi-Api-Key
  sources:
  - openapi/heidi-health-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/heidi-health-openapi.yml
  type: http
slug: heidi-health-authentication
source_filename: heidi-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heidi-health-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: heidiApiKey\n  type: apiKey\n  in: header\n  parameter: Heidi-Api-Key\n  sources:\n  - openapi/heidi-health-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/heidi-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/authentication/heidi-health-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Healthcare
- Health Tech
- AI Medical Scribe
- Ambient AI
- Clinical Documentation
- Clinical Decision Support
- Artificial Intelligence
- Speech To Text
- Transcription
- EHR Integration
- Electronic Health Records
- Telehealth
- Clinical Coding
- ICD-10
- SNOMED
- HIPAA
- GDPR
- SOC 2
- ISO 27001
- ISO 42001
- Wearables
- Voice
- Audio
- Australia
- Melbourne
---
