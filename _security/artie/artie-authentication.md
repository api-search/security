---
api_key_in:
- header
api_specs:
- filename: artie-openapi-original.yml
  format: yaml
  label: Artie API
  slug: artie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Artie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artie secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Artie
provider_slug: artie
scheme_count: 1
schemes:
- description: 'API key passed as a Bearer token in the Authorization header (Authorization: Bearer <key>). Keys are generated from the Artie dashboard and exposed to the CLI via the ARTIE_API_KEY environment variable.'
  env: ARTIE_API_KEY
  header: Authorization
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/artie-openapi-original.yml
  type: http
slug: artie-authentication
source_filename: artie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/artie-openapi-original.yml\ndocs: https://www.artie.com/docs/api-reference\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    API key passed as a Bearer token in the Authorization header\n    (Authorization: Bearer <key>). Keys are generated from the Artie dashboard\n    and exposed to the CLI via the ARTIE_API_KEY environment variable.\n  header: Authorization\n  env: ARTIE_API_KEY\n  sources:\n  - openapi/artie-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/authentication/artie-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Replication
- Change Data Capture
- Data Integration
- ETL
- Streaming
- Databases
- Data Warehouse
- CDC
- Data Engineering
---
