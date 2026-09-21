---
anonymous_access: false
api_key_in: []
api_specs:
- filename: schemaextract-openapi.yml
  format: yaml
  label: SchemaExtract API
  slug: schemaextract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemaextract/refs/heads/main/openapi/schemaextract-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Schemaextract Authentication
name_suffix: Authentication
oauth_flows: []
overview: SchemaExtract secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SchemaExtract
provider_slug: schemaextract
scheme_count: 1
schemes:
- bearerFormat: sk_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/schemaextract-openapi.yml
  type: http
slug: schemaextract-authentication
source_filename: schemaextract-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: openapi/schemaextract-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_live_\n  sources:\n  - openapi/schemaextract-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schemaextract/refs/heads/main/authentication/schemaextract-authentication.yml
summary_line: http · 1 scheme
tags:
- Document AI
- IDP
- Data Extraction
- PDF/OCR-to-JSON
- Invoice & AP automation
- Logistics/freight
- Fintech
- Developer API
---
