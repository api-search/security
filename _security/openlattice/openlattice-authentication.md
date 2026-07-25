---
api_key_in:
- header
api_specs:
- filename: openlattice-authorizations-api-openapi.yml
  format: yaml
  label: OpenLattice authorizations API
  slug: openlattice-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-authorizations-api-openapi.yml
- filename: openlattice-data-api-openapi.yml
  format: yaml
  label: OpenLattice data API
  slug: openlattice-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-data-api-openapi.yml
- filename: openlattice-edm-api-openapi.yml
  format: yaml
  label: OpenLattice edm API
  slug: openlattice-edm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-edm-api-openapi.yml
- filename: openlattice-organizations-api-openapi.yml
  format: yaml
  label: OpenLattice organizations API
  slug: openlattice-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-organizations-api-openapi.yml
- filename: openlattice-permissions-api-openapi.yml
  format: yaml
  label: OpenLattice permissions API
  slug: openlattice-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-permissions-api-openapi.yml
- filename: openlattice-principal-api-openapi.yml
  format: yaml
  label: OpenLattice principal API
  slug: openlattice-principal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-principal-api-openapi.yml
- filename: openlattice-search-api-openapi.yml
  format: yaml
  label: OpenLattice search API
  slug: openlattice-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-search-api-openapi.yml
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
