---
api_key_in: []
api_specs:
- filename: staples-advantage-eprocurement-api-openapi.yml
  format: yaml
  label: Staples Advantage eProcurement API
  slug: staples-advantage-eprocurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/staples/refs/heads/main/openapi/staples-advantage-eprocurement-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Staples Authentication
name_suffix: Authentication
oauth_flows: []
overview: Staples secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Staples
provider_slug: staples
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/staples-advantage-eprocurement-api-openapi.yml
  type: http
slug: staples-authentication
source_filename: staples-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/staples-advantage-eprocurement-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/staples-advantage-eprocurement-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/staples/refs/heads/main/authentication/staples-authentication.yml
summary_line: http · 1 scheme
tags:
- Office Supplies
- Retail
- Procurement
- B2B
- eProcurement
- Fortune 500
---
