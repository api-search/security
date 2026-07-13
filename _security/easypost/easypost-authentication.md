---
api_key_in: []
api_specs:
- filename: easypost-openapi.yml
  format: yaml
  label: EasyPost Shipping API
  slug: shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easypost/refs/heads/main/openapi/easypost-openapi.yml
- filename: easypost-webhooks-asyncapi.yml
  format: yaml
  label: EasyPost Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/easypost/refs/heads/main/asyncapi/easypost-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Easypost Authentication
name_suffix: Authentication
oauth_flows: []
overview: EasyPost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EasyPost
provider_slug: easypost
scheme_count: 1
schemes:
- description: HTTP Basic where username is your EasyPost API key and password is empty.
  name: EasyPostBasic
  scheme: basic
  sources:
  - openapi/easypost-openapi.yml
  type: http
slug: easypost-authentication
source_filename: easypost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/easypost-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: EasyPostBasic\n  type: http\n  scheme: basic\n  description: HTTP Basic where username is your EasyPost API key and password is empty.\n  sources:\n  - openapi/easypost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easypost/refs/heads/main/authentication/easypost-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Logistics
- Multi-Carrier
- Tracking
- Labels
- Insurance
---
