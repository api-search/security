---
api_key_in: []
api_specs:
- filename: fieldwire-account-api-openapi.yml
  format: yaml
  label: Fieldwire Account API
  slug: fieldwire-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-account-api-openapi.yml
- filename: fieldwire-projects-api-openapi.yml
  format: yaml
  label: Fieldwire Projects API
  slug: fieldwire-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-projects-api-openapi.yml
- filename: fieldwire-tasks-api-openapi.yml
  format: yaml
  label: Fieldwire Tasks API
  slug: fieldwire-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-tasks-api-openapi.yml
- filename: fieldwire-plans-api-openapi.yml
  format: yaml
  label: Fieldwire Plans and Sheets API
  slug: fieldwire-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-plans-api-openapi.yml
- filename: fieldwire-forms-api-openapi.yml
  format: yaml
  label: Fieldwire Forms API
  slug: fieldwire-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-forms-api-openapi.yml
- filename: fieldwire-attachments-api-openapi.yml
  format: yaml
  label: Fieldwire Attachments and Media API
  slug: fieldwire-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-attachments-api-openapi.yml
- filename: fieldwire-financials-api-openapi.yml
  format: yaml
  label: Fieldwire Project Financials API
  slug: fieldwire-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-financials-api-openapi.yml
- filename: fieldwire-rfis-submittals-api-openapi.yml
  format: yaml
  label: Fieldwire RFIs and Submittals API
  slug: fieldwire-rfis-submittals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-rfis-submittals-api-openapi.yml
- filename: fieldwire-webhooks-api-openapi.yml
  format: yaml
  label: Fieldwire Webhooks API
  slug: fieldwire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fieldwire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fieldwire secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fieldwire
provider_slug: fieldwire
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Send the short-lived access token returned by `POST /api_keys/jwt` as

    `Authorization: Bearer <access_token>`. Also include the

    `Fieldwire-Version` request header and `Content-Type: application/json`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fieldwire-account-api-openapi.yml
  - openapi/fieldwire-attachments-api-openapi.yml
  - openapi/fieldwire-financials-api-openapi.yml
  - openapi/fieldwire-forms-api-openapi.yml
  - openapi/fieldwire-plans-api-openapi.yml
  - openapi/fieldwire-projects-api-openapi.yml
  - openapi/fieldwire-rfis-submittals-api-openapi.yml
  - openapi/fieldwire-tasks-api-openapi.yml
  - openapi/fieldwire-webhooks-api-openapi.yml
  type: http
slug: fieldwire-authentication
source_filename: fieldwire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fieldwire-account-api-openapi.yml, openapi/fieldwire-attachments-api-openapi.yml,\n  openapi/fieldwire-financials-api-openapi.yml, openapi/fieldwire-forms-api-openapi.yml, openapi/fieldwire-plans-api-openapi.yml,\n  openapi/fieldwire-projects-api-openapi.yml, openapi/fieldwire-rfis-submittals-api-openapi.yml,\n  openapi/fieldwire-tasks-api-openapi.yml, openapi/fieldwire-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Send the short-lived access token returned by `POST /api_keys/jwt` as\n    `Authorization: Bearer <access_token>`. Also include the\n    `Fieldwire-Version` request header and `Content-Type: application/json`.\n  sources:\n  - openapi/fieldwire-account-api-openapi.yml\n  - openapi/fieldwire-attachments-api-openapi.yml\n  - openapi/fieldwire-financials-api-openapi.yml\n  - openapi/fieldwire-forms-api-openapi.yml\n\
  \  - openapi/fieldwire-plans-api-openapi.yml\n  - openapi/fieldwire-projects-api-openapi.yml\n  - openapi/fieldwire-rfis-submittals-api-openapi.yml\n  - openapi/fieldwire-tasks-api-openapi.yml\n  - openapi/fieldwire-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/authentication/fieldwire-authentication.yml
summary_line: http · 1 scheme
tags:
- Construction
- Construction Technology
- ConTech
- Field Management
- Punch List
- Plans
- Drawings
- BIM
- Forms
- Inspections
- Project Management
- Hilti
---
