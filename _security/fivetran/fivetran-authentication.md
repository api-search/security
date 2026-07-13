---
api_key_in: []
api_specs:
- filename: fivetran-openapi.yml
  format: yaml
  label: Fivetran REST API
  slug: fivetran-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fivetran Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fivetran secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fivetran
provider_slug: fivetran
scheme_count: 1
schemes:
- description: HTTP Basic auth using `<api_key>:<api_secret>`
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fivetran-openapi.yml
  type: http
slug: fivetran-authentication
source_filename: fivetran-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fivetran-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using `<api_key>:<api_secret>`\n  sources:\n  - openapi/fivetran-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/authentication/fivetran-authentication.yml
summary_line: http · 1 scheme
tags:
- Connectors
- Data Integration
- Data Pipeline
- ETL
- SaaS
- Unified API
---
