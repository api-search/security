---
api_key_in:
- header
api_specs:
- filename: odoo-openapi.yml
  format: yaml
  label: Odoo External API
  slug: odoo-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odoo/refs/heads/main/openapi/odoo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Odoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Odoo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Odoo
provider_slug: odoo
scheme_count: 1
schemes:
- description: 'Odoo 14+ supports per-user API keys generated under user preferences

    Account Security. These can be substituted for the password parameter

    in `authenticate` and `execute_kw` calls.'
  in: header
  name: OdooApiKey
  parameter: X-API-Key
  sources:
  - openapi/odoo-openapi.yml
  type: apiKey
slug: odoo-authentication
source_filename: odoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/odoo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OdooApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    Odoo 14+ supports per-user API keys generated under user preferences\n    Account Security. These can be substituted for the password parameter\n    in `authenticate` and `execute_kw` calls.\n  sources:\n  - openapi/odoo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odoo/refs/heads/main/authentication/odoo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Applications
- CRM
- ERP
- Open Source
---
