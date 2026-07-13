---
api_key_in: []
api_specs:
- filename: agile-crm-openapi.yml
  format: yaml
  label: Agile CRM REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-openapi.yml
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
