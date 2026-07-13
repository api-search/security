---
api_key_in: []
api_specs:
- filename: tripetto-form-builder-openapi.yml
  format: yaml
  label: Tripetto FormBuilder SDK
  slug: tripetto-form-builder-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripetto/refs/heads/main/openapi/tripetto-form-builder-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tripetto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tripetto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tripetto
provider_slug: tripetto
scheme_count: 1
schemes:
- description: Bearer token for API authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tripetto-form-builder-openapi.yml
  type: http
slug: tripetto-authentication
source_filename: tripetto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tripetto-form-builder-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for API authentication\n  sources:\n  - openapi/tripetto-form-builder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripetto/refs/heads/main/authentication/tripetto-authentication.yml
summary_line: http · 1 scheme
tags:
- Forms
- Surveys
- Form Builder
- No-Code
- SDK
- Webhooks
---
