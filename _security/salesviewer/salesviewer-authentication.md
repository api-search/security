---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: salesviewer-salesviewer-api-swagger-openapi.json
  format: json
  label: SalesViewer® Salesviewer Api.Swagger API
  slug: salesviewer-salesviewer-api-swagger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/salesviewer/openapi/_original/salesviewer-salesviewer-api-swagger-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: SalesViewer® Authentication
name_suffix: Authentication
oauth_flows: []
overview: SalesViewer® secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SalesViewer®
provider_slug: salesviewer
scheme_count: 2
schemes:
- description: Authentication for each request with api key in header data.
  in: header
  name: apiKeyHeader
  parameter: X-SV-APIKEY
  sources:
  - openapi/salesviewer-openapi.json
  type: apiKey
- description: Authentication for each request with api key in query.
  in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/salesviewer-openapi.json
  type: apiKey
slug: salesviewer-authentication
source_filename: salesviewer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/salesviewer-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-SV-APIKEY\n  description: Authentication for each request with api key in header data.\n  sources:\n  - openapi/salesviewer-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Authentication for each request with api key in query.\n  sources:\n  - openapi/salesviewer-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/salesviewer/authentication/salesviewer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Lead Generation
- B2B Sales
---
