---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Folk API
  slug: folk-api
  spec_type: OpenAPI
  url: https://developer.folk.app/api-reference/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Folk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Folk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Folk
provider_slug: folk
scheme_count: 1
schemes:
- description: API key for authentication
  name: bearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/folk-openapi.yml
  type: http
slug: folk-authentication
source_filename: folk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/folk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key for authentication\n  sources:\n  - openapi/folk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/authentication/folk-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Contacts
- Pipelines
- Sales
- Relationships
- Notes
- Deals
- Webhooks
---
