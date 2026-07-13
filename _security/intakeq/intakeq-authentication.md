---
api_key_in:
- header
api_specs:
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Clients API
  slug: intakeq-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Appointments API
  slug: intakeq-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Intake Forms API
  slug: intakeq-intake-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Treatment Notes API
  slug: intakeq-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Invoices API
  slug: intakeq-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Files API
  slug: intakeq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Intakeq Authentication
name_suffix: Authentication
oauth_flows: []
overview: IntakeQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IntakeQ
provider_slug: intakeq
scheme_count: 1
schemes:
- description: The account API key found under More > Settings > Integrations > Developer API.
  in: header
  name: authKey
  parameter: X-Auth-Key
  sources:
  - openapi/intakeq-openapi.yml
  type: apiKey
slug: intakeq-authentication
source_filename: intakeq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intakeq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  description: The account API key found under More > Settings > Integrations > Developer API.\n  sources:\n  - openapi/intakeq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/authentication/intakeq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Practice Management
- Intake Forms
- Scheduling
- Health and Wellness
- EHR
- Telehealth
- HIPAA
---
