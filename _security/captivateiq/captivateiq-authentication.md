---
api_key_in:
- header
api_specs:
- filename: captivateiq-openapi-original.yml
  format: yaml
  label: CaptivateIQ API
  slug: captivateiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Captivateiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaptivateIQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CaptivateIQ
provider_slug: captivateiq
scheme_count: 1
schemes:
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/captivateiq-openapi-original.yml
  type: apiKey
slug: captivateiq-authentication
source_filename: captivateiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/captivateiq-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/captivateiq-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/authentication/captivateiq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cloud Saas
- Sales Commissions
- Incentive Compensation Management
- Sales Performance Management
- Revenue Operations
- Finance
- Payouts
- Commission Plans
- Sales Compensation
---
