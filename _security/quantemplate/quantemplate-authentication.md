---
api_key_in: []
api_specs:
- filename: quantemplate-fabric-openapi.yml
  format: yaml
  label: Quantemplate FabricAPI
  slug: quantemplate-fabricapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quantemplate/refs/heads/main/openapi/quantemplate-fabric-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quantemplate Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuanTemplate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuanTemplate
provider_slug: quantemplate
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/quantemplate-fabric-openapi.yml
  type: http
slug: quantemplate-authentication
source_filename: quantemplate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/quantemplate-fabric-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/quantemplate-fabric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantemplate/refs/heads/main/authentication/quantemplate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Data Integration
- Data Management
- Bordereaux
- Data Validation
- Pipelines
- Analytics
- No-Code
- API
---
