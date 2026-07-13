---
api_key_in: []
api_specs:
- filename: dremio-intelligent-lakehouse-platform-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform
  slug: dremio-intelligent-lakehouse-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dremio Intelligent Lakehouse Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dremio | Intelligent Lakehouse Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dremio | Intelligent Lakehouse Platform
provider_slug: dremio-intelligent-lakehouse-platform
scheme_count: 1
schemes:
- description: OAuth access token or Personal Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dremio-intelligent-lakehouse-platform-openapi.yml
  type: http
slug: dremio-intelligent-lakehouse-platform-authentication
source_filename: dremio-intelligent-lakehouse-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dremio-intelligent-lakehouse-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth access token or Personal Access Token\n  sources:\n  - openapi/dremio-intelligent-lakehouse-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/authentication/dremio-intelligent-lakehouse-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Analytics
- Lakehouse
- Apache Iceberg
- SQL
- AI
---
