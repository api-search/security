---
api_key_in:
- header
api_specs:
- filename: holded-openapi.yml
  format: yaml
  label: Holded REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Holded Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holded secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Holded
provider_slug: holded
scheme_count: 1
schemes:
- description: Holded tenant API key, generated in account settings.
  in: header
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/holded-openapi.yml
  type: apiKey
slug: holded-authentication
source_filename: holded-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/holded-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: Holded tenant API key, generated in account settings.\n  sources:\n  - openapi/holded-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/authentication/holded-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP
- CRM
- Accounting
- Invoicing
- Business Management
- SMB
- Spain
---
