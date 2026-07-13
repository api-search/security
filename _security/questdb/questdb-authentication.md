---
api_key_in: []
api_specs:
- filename: questdb-openapi.yml
  format: yaml
  label: QuestDB HTTP REST API
  slug: rest-http
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/questdb/refs/heads/main/openapi/questdb-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Questdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuestDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuestDB
provider_slug: questdb
scheme_count: 1
schemes:
- description: HTTP Basic Authentication (QuestDB Enterprise).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/questdb-openapi.yml
  type: http
slug: questdb-authentication
source_filename: questdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/questdb-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication (QuestDB Enterprise).\n  sources:\n  - openapi/questdb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/questdb/refs/heads/main/authentication/questdb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- Time-Series
- SQL
- Open Source
- Performance
- ILP
- PostgreSQL
---
