---
api_key_in: []
api_specs:
- filename: filevine-identity-api-openapi.yml
  format: yaml
  label: Filevine Identity API
  slug: filevine-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-identity-api-openapi.yml
- filename: filevine-projects-api-openapi.yml
  format: yaml
  label: Filevine Projects API
  slug: filevine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-projects-api-openapi.yml
- filename: filevine-contacts-api-openapi.yml
  format: yaml
  label: Filevine Contacts API
  slug: filevine-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-contacts-api-openapi.yml
- filename: filevine-documents-api-openapi.yml
  format: yaml
  label: Filevine Documents API
  slug: filevine-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-documents-api-openapi.yml
- filename: filevine-notes-api-openapi.yml
  format: yaml
  label: Filevine Notes API
  slug: filevine-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-notes-api-openapi.yml
- filename: filevine-deadlines-api-openapi.yml
  format: yaml
  label: Filevine Deadlines API
  slug: filevine-deadlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-deadlines-api-openapi.yml
- filename: filevine-tasks-api-openapi.yml
  format: yaml
  label: Filevine Tasks API
  slug: filevine-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-tasks-api-openapi.yml
- filename: filevine-time-entries-api-openapi.yml
  format: yaml
  label: Filevine Time Entries API
  slug: filevine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-time-entries-api-openapi.yml
- filename: filevine-webhooks-api-openapi.yml
  format: yaml
  label: Filevine Webhooks API
  slug: filevine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Filevine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filevine secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Filevine
provider_slug: filevine
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/filevine-contacts-api-openapi.yml
  - openapi/filevine-deadlines-api-openapi.yml
  - openapi/filevine-documents-api-openapi.yml
  - openapi/filevine-notes-api-openapi.yml
  - openapi/filevine-projects-api-openapi.yml
  - openapi/filevine-tasks-api-openapi.yml
  - openapi/filevine-time-entries-api-openapi.yml
  - openapi/filevine-webhooks-api-openapi.yml
  type: http
slug: filevine-authentication
source_filename: filevine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/filevine-contacts-api-openapi.yml, openapi/filevine-deadlines-api-openapi.yml,\n  openapi/filevine-documents-api-openapi.yml, openapi/filevine-notes-api-openapi.yml, openapi/filevine-projects-api-openapi.yml,\n  openapi/filevine-tasks-api-openapi.yml, openapi/filevine-time-entries-api-openapi.yml, openapi/filevine-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/filevine-contacts-api-openapi.yml\n  - openapi/filevine-deadlines-api-openapi.yml\n  - openapi/filevine-documents-api-openapi.yml\n  - openapi/filevine-notes-api-openapi.yml\n  - openapi/filevine-projects-api-openapi.yml\n  - openapi/filevine-tasks-api-openapi.yml\n  - openapi/filevine-time-entries-api-openapi.yml\n  - openapi/filevine-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/authentication/filevine-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal
- Case Management
- Matters
- Intake
- Documents
- LOIS
- Webhooks
- Legal AI
- Personal Injury
- Mass Torts
---
