---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: CData secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CData
provider_slug: cdata
scheme_count: 2
schemes:
- description: Basic auth using CData Connect Cloud username and PAT/password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cdata-openapi.yml
  type: http
- bearerFormat: JWT
  description: JWT bearer for CData Connect AI Embed
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cdata-openapi.yml
  type: http
slug: cdata-authentication
source_filename: cdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cdata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic auth using CData Connect Cloud username and PAT/password\n  sources:\n  - openapi/cdata-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer for CData Connect AI Embed\n  sources:\n  - openapi/cdata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/authentication/cdata-authentication.yml
summary_line: http · 2 schemes
tags:
- Data
- Data Access
- Data Connectivity
- Databases
- NoSQL
- SQL
---
