---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Innago API
  slug: innago-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Innago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Innago secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Innago
provider_slug: innago
scheme_count: 2
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: innago-authentication
source_filename: innago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innago/refs/heads/main/authentication/innago-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Property Management
- Real Estate
- Leases
- Rent Collection
- Maintenance
- Tenants
- Invoicing
- Payments
---
