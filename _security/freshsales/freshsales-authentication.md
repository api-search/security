---
api_key_in:
- header
api_specs:
- filename: freshsales-appointments-api-openapi.yml
  format: yaml
  label: Freshsales Appointments API
  slug: freshsales-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-appointments-api-openapi.yml
- filename: freshsales-calls-api-openapi.yml
  format: yaml
  label: Freshsales Calls API
  slug: freshsales-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-calls-api-openapi.yml
- filename: freshsales-contacts-api-openapi.yml
  format: yaml
  label: Freshsales Contacts API
  slug: freshsales-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-contacts-api-openapi.yml
- filename: freshsales-deals-api-openapi.yml
  format: yaml
  label: Freshsales Deals API
  slug: freshsales-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-deals-api-openapi.yml
- filename: freshsales-jobs-api-openapi.yml
  format: yaml
  label: Freshsales Jobs API
  slug: freshsales-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-jobs-api-openapi.yml
- filename: freshsales-lists-api-openapi.yml
  format: yaml
  label: Freshsales Lists API
  slug: freshsales-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-lists-api-openapi.yml
- filename: freshsales-notes-api-openapi.yml
  format: yaml
  label: Freshsales Notes API
  slug: freshsales-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-notes-api-openapi.yml
- filename: freshsales-products-api-openapi.yml
  format: yaml
  label: Freshsales Products API
  slug: freshsales-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-products-api-openapi.yml
- filename: freshsales-salesaccounts-api-openapi.yml
  format: yaml
  label: Freshsales SalesAccounts API
  slug: freshsales-salesaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-salesaccounts-api-openapi.yml
- filename: freshsales-salesactivities-api-openapi.yml
  format: yaml
  label: Freshsales SalesActivities API
  slug: freshsales-salesactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-salesactivities-api-openapi.yml
- filename: freshsales-search-api-openapi.yml
  format: yaml
  label: Freshsales Search API
  slug: freshsales-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-search-api-openapi.yml
- filename: freshsales-tasks-api-openapi.yml
  format: yaml
  label: Freshsales Tasks API
  slug: freshsales-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/openapi/freshsales-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freshsales Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshsales secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshsales
provider_slug: freshsales
scheme_count: 1
schemes:
- description: 'Token-based authentication header in the form

    "Authorization: Token token=YOUR_API_KEY".'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/freshsales-openapi.yml
  type: apiKey
slug: freshsales-authentication
source_filename: freshsales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshsales-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Token-based authentication header in the form\n    \"Authorization: Token token=YOUR_API_KEY\".\n  sources:\n  - openapi/freshsales-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshsales/refs/heads/main/authentication/freshsales-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- Sales
- Contacts
- Deals
- Pipeline
- Lead Management
- Freshworks
---
