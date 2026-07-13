---
api_key_in: []
api_specs:
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Patients API
  slug: cliniko-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointments API
  slug: cliniko-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Practitioners and Businesses API
  slug: cliniko-practitioners-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointment Types API
  slug: cliniko-appointment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Invoices API
  slug: cliniko-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Treatment Notes API
  slug: cliniko-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cliniko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cliniko secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cliniko
provider_slug: cliniko
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication over HTTPS. The Cliniko API key is supplied as the username and the password is left empty (curl: `-u API_KEY:`). Construct the header as `Authorization: Basic ` + base64(api_key + ":"). API keys are generated per user in Cliniko under "My Info". The shard suffix on the key (for example `-uk1`) selects the base host, e.g. https://api.uk1.cliniko.com; keys with no suffix belong to the au1 shard. Every request must also send `Accept: application/json` and a `User-Agent` header of the form `APP_VENDOR_NAME (APP_VENDOR_EMAIL)` with a valid contact email, or requests may be automatically blocked.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cliniko-openapi.yml
  - https://docs.api.cliniko.com/
  - https://github.com/redguava/cliniko-api
  type: http
slug: cliniko-authentication
source_filename: cliniko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/cliniko-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication over HTTPS. The Cliniko API key is supplied as the\n    username and the password is left empty (curl: `-u API_KEY:`). Construct the\n    header as `Authorization: Basic ` + base64(api_key + \":\"). API keys are\n    generated per user in Cliniko under \"My Info\". The shard suffix on the key\n    (for example `-uk1`) selects the base host, e.g. https://api.uk1.cliniko.com;\n    keys with no suffix belong to the au1 shard. Every request must also send\n    `Accept: application/json` and a `User-Agent` header of the form\n    `APP_VENDOR_NAME (APP_VENDOR_EMAIL)` with a valid contact email, or requests\n    may be automatically blocked.\n  sources:\n  - openapi/cliniko-openapi.yml\n  - https://docs.api.cliniko.com/\n  - https://github.com/redguava/cliniko-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/authentication/cliniko-authentication.yml
summary_line: http · 1 scheme
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- EHR
- Clinics
- Bookings
- SaaS
---
