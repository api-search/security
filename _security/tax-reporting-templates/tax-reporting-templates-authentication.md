---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tax Reporting Templates Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tax Reporting Templates secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tax Reporting Templates
provider_slug: tax-reporting-templates
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tax-reporting-templates-openapi.yml
  type: http
slug: tax-reporting-templates-authentication
source_filename: tax-reporting-templates-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tax-reporting-templates-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/tax-reporting-templates-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tax-reporting-templates/refs/heads/main/authentication/tax-reporting-templates-authentication.yml
summary_line: http · 1 scheme
tags:
- Compliance
- Documentation
- Finance
- Reporting
- Tax
- Templates
---
