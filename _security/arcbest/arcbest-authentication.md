---
api_key_in: []
api_specs:
- filename: arcbest-api.yaml
  format: yaml
  label: ArcBest API
  slug: arcbest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arcbest Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArcBest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ArcBest
provider_slug: arcbest
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained from ArcBest API authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcbest-api.yaml
  type: http
slug: arcbest-authentication
source_filename: arcbest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcbest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from ArcBest API authentication\n  sources:\n  - openapi/arcbest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/authentication/arcbest-authentication.yml
summary_line: http · 1 scheme
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
---
