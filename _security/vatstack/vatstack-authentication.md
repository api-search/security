---
api_key_in:
- header
api_specs:
- filename: openapi
  format: yaml
  label: Vatstack API
  slug: vatstack-api
  spec_type: OpenAPI
  url: https://github.com/vatstack/openapi
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vatstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vatstack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vatstack
provider_slug: vatstack
scheme_count: 1
schemes:
- in: header
  name: publicKey
  parameter: X-API-KEY
  sources:
  - openapi/vatstack-openapi.json
  type: apiKey
slug: vatstack-authentication
source_filename: vatstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vatstack-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: publicKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/vatstack-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/authentication/vatstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- VAT
- Tax
- Validation
- EU
- Europe
- Compliance
- Finance
- Business
---
