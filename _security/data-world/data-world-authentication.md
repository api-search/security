---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: data.world REST API
  slug: dataworld-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-world/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Data World Authentication
name_suffix: Authentication
oauth_flows: []
overview: data.world secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: data.world
provider_slug: data-world
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: data-world-authentication
source_filename: data-world-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-world/refs/heads/main/authentication/data-world-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Catalog
- Data Governance
- Metadata Management
- SPARQL
- SQL
- Open Data
- Collaboration
---
