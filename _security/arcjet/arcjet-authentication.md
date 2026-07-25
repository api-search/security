---
api_key_in:
- header
api_specs:
- filename: arcjet-decide-api-openapi.yml
  format: yaml
  label: Arcjet Decide API
  slug: arcjet-decide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-decide-api-openapi.yml
- filename: arcjet-report-api-openapi.yml
  format: yaml
  label: Arcjet Report API
  slug: arcjet-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/openapi/arcjet-report-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arcjet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcjet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcjet
provider_slug: arcjet
scheme_count: 1
schemes:
- description: Arcjet site key, supplied by the SDK from the ARCJET_KEY environment variable.
  in: header
  name: arcjetKey
  parameter: Authorization
  sources:
  - openapi/arcjet-openapi.yml
  type: apiKey
slug: arcjet-authentication
source_filename: arcjet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcjet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: arcjetKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Arcjet site key, supplied by the SDK from the ARCJET_KEY environment variable.\n  sources:\n  - openapi/arcjet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcjet/refs/heads/main/authentication/arcjet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Rate Limiting
- Bot Detection
- WAF
- Developer Security
---
