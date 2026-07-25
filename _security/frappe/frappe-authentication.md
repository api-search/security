---
api_key_in:
- header
api_specs:
- filename: frappe-method-api-openapi.yml
  format: yaml
  label: Frappe Method API
  slug: frappe-method-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/openapi/frappe-method-api-openapi.yml
- filename: frappe-resource-api-openapi.yml
  format: yaml
  label: Frappe Resource API
  slug: frappe-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/openapi/frappe-resource-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Frappe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frappe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Frappe
provider_slug: frappe
scheme_count: 1
schemes:
- description: token <api_key>:<api_secret>
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/frappe-openapi.yml
  type: apiKey
slug: frappe-authentication
source_filename: frappe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/frappe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: token <api_key>:<api_secret>\n  sources:\n  - openapi/frappe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frappe/refs/heads/main/authentication/frappe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Source
- ERP
- Accounting
- Inventory
- Payroll
- Low Code
---
