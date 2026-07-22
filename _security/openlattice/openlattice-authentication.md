---
api_key_in:
- header
api_specs:
- filename: openlattice-openapi.yaml
  format: yaml
  label: OpenLattice API
  slug: openlattice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openlattice Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenLattice secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenLattice
provider_slug: openlattice
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: http_auth
  scheme: bearer
  sources:
  - openapi/openlattice-openapi.yaml
  type: http
- in: header
  name: openlattice_auth
  parameter: Authorization
  sources:
  - openapi/openlattice-openapi.yaml
  type: apiKey
slug: openlattice-authentication
source_filename: openlattice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/openlattice-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: http_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openlattice-openapi.yaml\n- name: openlattice_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openlattice-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/authentication/openlattice-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Data Integration
- Entity Data Model
- Public Sector
- Analytics
- Graph
- Criminal Justice
---
