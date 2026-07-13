---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: NocoDB Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://app.nocodb.com/api/v3/swagger.json
- filename: swagger.json
  format: json
  label: NocoDB Meta API
  slug: meta-api
  spec_type: OpenAPI
  url: https://app.nocodb.com/api/v2/meta/bases/{base_id}/swagger.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nocodb Authentication
name_suffix: Authentication
oauth_flows: []
overview: NocoDB secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NocoDB
provider_slug: nocodb
scheme_count: 2
schemes:
- description: NocoDB API token
  in: header
  name: xcToken
  parameter: xc-token
  sources:
  - openapi/nocodb-data-api-openapi.yml
  - openapi/nocodb-meta-api-openapi.yml
  type: apiKey
- description: 'Bearer token authentication. Use ''Authorization: Bearer <token>'' header format.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nocodb-data-api-openapi.yml
  - openapi/nocodb-meta-api-openapi.yml
  type: http
slug: nocodb-authentication
source_filename: nocodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nocodb-data-api-openapi.yml, openapi/nocodb-meta-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: xcToken\n  type: apiKey\n  in: header\n  parameter: xc-token\n  description: NocoDB API token\n  sources:\n  - openapi/nocodb-data-api-openapi.yml\n  - openapi/nocodb-meta-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication. Use ''Authorization: Bearer <token>'' header format.'\n  sources:\n  - openapi/nocodb-data-api-openapi.yml\n  - openapi/nocodb-meta-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nocodb/refs/heads/main/authentication/nocodb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Database
- No-Code
- Low-Code
- Airtable Alternative
- Open Source
- Spreadsheet
- REST API
- Self-Hosted
---
