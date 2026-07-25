---
api_key_in: []
api_specs:
- filename: agile-crm-campaigns-api-openapi.yml
  format: yaml
  label: Agile CRM Campaigns API
  slug: agile-crm-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-campaigns-api-openapi.yml
- filename: agile-crm-companies-api-openapi.yml
  format: yaml
  label: Agile CRM Companies API
  slug: agile-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-companies-api-openapi.yml
- filename: agile-crm-contacts-api-openapi.yml
  format: yaml
  label: Agile CRM Contacts API
  slug: agile-crm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-contacts-api-openapi.yml
- filename: agile-crm-deals-api-openapi.yml
  format: yaml
  label: Agile CRM Deals API
  slug: agile-crm-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-deals-api-openapi.yml
- filename: agile-crm-documents-api-openapi.yml
  format: yaml
  label: Agile CRM Documents API
  slug: agile-crm-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-documents-api-openapi.yml
- filename: agile-crm-events-api-openapi.yml
  format: yaml
  label: Agile CRM Events API
  slug: agile-crm-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-events-api-openapi.yml
- filename: agile-crm-helpdesk-api-openapi.yml
  format: yaml
  label: Agile CRM HelpDesk API
  slug: agile-crm-helpdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-helpdesk-api-openapi.yml
- filename: agile-crm-notes-api-openapi.yml
  format: yaml
  label: Agile CRM Notes API
  slug: agile-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-notes-api-openapi.yml
- filename: agile-crm-tasks-api-openapi.yml
  format: yaml
  label: Agile CRM Tasks API
  slug: agile-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-tasks-api-openapi.yml
- filename: agile-crm-tracks-api-openapi.yml
  format: yaml
  label: Agile CRM Tracks API
  slug: agile-crm-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-tracks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agile Crm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agile CRM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agile CRM
provider_slug: agile-crm
scheme_count: 1
schemes:
- description: HTTP Basic auth - username is account email, password is REST client API key.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/agile-crm-openapi.yml
  type: http
slug: agile-crm-authentication
source_filename: agile-crm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agile-crm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth - username is account email, password is REST client API key.\n  sources:\n  - openapi/agile-crm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/authentication/agile-crm-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Sales Automation
- Marketing Automation
- Helpdesk
- Small Business
- Contact Management
---
