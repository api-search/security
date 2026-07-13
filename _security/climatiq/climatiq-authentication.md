---
api_key_in: []
api_specs:
- filename: climatiq-openapi.yml
  format: yaml
  label: Climatiq API
  slug: climatiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Climatiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Climatiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Climatiq
provider_slug: climatiq
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/climatiq-openapi.yml
  type: http
slug: climatiq-authentication
source_filename: climatiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/climatiq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/climatiq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/authentication/climatiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Energy
- Environment
- GHG Protocol
- Sustainability
---
