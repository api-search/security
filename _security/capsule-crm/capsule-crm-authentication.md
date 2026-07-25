---
api_key_in: []
api_specs:
- filename: capsule-crm-entries-api-openapi.yml
  format: yaml
  label: Capsule CRM Entries API
  slug: capsule-crm-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-entries-api-openapi.yml
- filename: capsule-crm-opportunities-api-openapi.yml
  format: yaml
  label: Capsule CRM Opportunities API
  slug: capsule-crm-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-opportunities-api-openapi.yml
- filename: capsule-crm-parties-api-openapi.yml
  format: yaml
  label: Capsule CRM Parties API
  slug: capsule-crm-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-parties-api-openapi.yml
- filename: capsule-crm-projects-api-openapi.yml
  format: yaml
  label: Capsule CRM Projects API
  slug: capsule-crm-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-projects-api-openapi.yml
- filename: capsule-crm-tasks-api-openapi.yml
  format: yaml
  label: Capsule CRM Tasks API
  slug: capsule-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/openapi/capsule-crm-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Capsule Crm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capsule CRM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capsule CRM
provider_slug: capsule-crm
scheme_count: 1
schemes:
- description: Personal access token or OAuth 2 access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/capsule-crm-openapi.yml
  type: http
slug: capsule-crm-authentication
source_filename: capsule-crm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/capsule-crm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token or OAuth 2 access token\n  sources:\n  - openapi/capsule-crm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule-crm/refs/heads/main/authentication/capsule-crm-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Sales
- Contacts
- Pipeline Management
- Tasks
- Projects
- SMB
---
