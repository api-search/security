---
api_key_in:
- header
api_specs:
- filename: export-import-bank-of-the-united-states-openapi.yml
  format: yaml
  label: EXIM Open Data API
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/about-exim-exim-gov-export-import-bank-of-the-united-states/refs/heads/main/openapi/export-import-bank-of-the-united-states-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Export Import Bank Of The United States Authentication
name_suffix: Authentication
oauth_flows: []
overview: Export-Import Bank of the United States secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Export-Import Bank of the United States
provider_slug: about-exim-exim-gov-export-import-bank-of-the-united-states
scheme_count: 1
schemes:
- description: 'Optional Socrata application token. Unauthenticated requests

    are subject to lower throttling limits.'
  in: header
  name: AppToken
  parameter: X-App-Token
  sources:
  - openapi/export-import-bank-of-the-united-states-openapi.yml
  type: apiKey
slug: export-import-bank-of-the-united-states-authentication
source_filename: export-import-bank-of-the-united-states-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/export-import-bank-of-the-united-states-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: |-\n    Optional Socrata application token. Unauthenticated requests\n    are subject to lower throttling limits.\n  sources:\n  - openapi/export-import-bank-of-the-united-states-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/about-exim-exim-gov-export-import-bank-of-the-united-states/refs/heads/main/authentication/export-import-bank-of-the-united-states-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Export
- Federal Government
- Finance
- Import
- Trade Finance
---
