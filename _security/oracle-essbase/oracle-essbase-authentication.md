---
api_key_in: []
api_specs:
- filename: oracle-essbase-rest-api-openapi.yml
  format: yaml
  label: Oracle Essbase REST API
  slug: oracle-essbase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Essbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Essbase secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Essbase
provider_slug: oracle-essbase
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using Essbase username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-essbase-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token authentication for cloud deployments on Oracle Cloud Infrastructure.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-essbase-rest-api-openapi.yml
  type: http
slug: oracle-essbase-authentication
source_filename: oracle-essbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-essbase-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Essbase username and password.\n  sources:\n  - openapi/oracle-essbase-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token authentication for cloud deployments on Oracle Cloud Infrastructure.\n  sources:\n  - openapi/oracle-essbase-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/authentication/oracle-essbase-authentication.yml
summary_line: http · 2 schemes
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
---
