---
api_key_in: []
api_specs:
- filename: qlik-cloud-openapi.yml
  format: yaml
  label: Qlik Cloud REST API
  slug: qlik-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-cloud/refs/heads/main/openapi/qlik-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qlik Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qlik Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qlik Cloud
provider_slug: qlik-cloud
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qlik-cloud-openapi.yml
  type: http
slug: qlik-cloud-authentication
source_filename: qlik-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qlik-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/qlik-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik-cloud/refs/heads/main/authentication/qlik-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Business Intelligence
- Cloud
- Data Integration
- SaaS
- Visualization
---
