---
api_key_in:
- header
api_specs:
- filename: revert-accounting-api-openapi.yml
  format: yaml
  label: Revert Accounting API
  slug: revert-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-accounting-api-openapi.yml
- filename: revert-chat-api-openapi.yml
  format: yaml
  label: Revert Chat API
  slug: revert-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-chat-api-openapi.yml
- filename: revert-connections-api-openapi.yml
  format: yaml
  label: Revert Connections API
  slug: revert-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-connections-api-openapi.yml
- filename: revert-crm-companies-api-openapi.yml
  format: yaml
  label: Revert CRM Companies API
  slug: revert-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-companies-api-openapi.yml
- filename: revert-crm-contacts-api-openapi.yml
  format: yaml
  label: Revert CRM Contacts API
  slug: revert-crm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-contacts-api-openapi.yml
- filename: revert-crm-deals-api-openapi.yml
  format: yaml
  label: Revert CRM Deals API
  slug: revert-crm-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-deals-api-openapi.yml
- filename: revert-crm-events-api-openapi.yml
  format: yaml
  label: Revert CRM Events API
  slug: revert-crm-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-events-api-openapi.yml
- filename: revert-crm-leads-api-openapi.yml
  format: yaml
  label: Revert CRM Leads API
  slug: revert-crm-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-leads-api-openapi.yml
- filename: revert-crm-notes-api-openapi.yml
  format: yaml
  label: Revert CRM Notes API
  slug: revert-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-notes-api-openapi.yml
- filename: revert-crm-properties-api-openapi.yml
  format: yaml
  label: Revert CRM Properties API
  slug: revert-crm-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-properties-api-openapi.yml
- filename: revert-crm-tasks-api-openapi.yml
  format: yaml
  label: Revert CRM Tasks API
  slug: revert-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-tasks-api-openapi.yml
- filename: revert-crm-users-api-openapi.yml
  format: yaml
  label: Revert CRM Users API
  slug: revert-crm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-users-api-openapi.yml
- filename: revert-tickets-api-openapi.yml
  format: yaml
  label: Revert Tickets API
  slug: revert-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-tickets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revert
provider_slug: revert
scheme_count: 1
schemes:
- description: Your official API key for accessing Revert APIs
  in: header
  name: ApiTokenAuth
  parameter: x-revert-api-token
  sources:
  - openapi/revert-unified-api-openapi.yml
  type: apiKey
slug: revert-authentication
source_filename: revert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revert-unified-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: x-revert-api-token\n  description: Your official API key for accessing Revert APIs\n  sources:\n  - openapi/revert-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/authentication/revert-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Integration
- CRM
- Unified-API
- Open-Source
---
