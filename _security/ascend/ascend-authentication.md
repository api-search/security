---
api_key_in: []
api_specs:
- filename: ascend-openapi-original.yml
  format: yaml
  label: Ascend API V1
  slug: ascend-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ascend/refs/heads/main/openapi/ascend-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ascend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ascend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ascend
provider_slug: ascend
scheme_count: 1
schemes:
- name: bearer_auth
  scheme: bearer
  sources:
  - openapi/ascend-openapi-original.yml
  type: http
slug: ascend-authentication
source_filename: ascend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/ascend-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ascend-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascend/refs/heads/main/authentication/ascend-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Insurance
- InsurTech
- Payments
- Premium Financing
- Billing
- Invoicing
- Embedded Finance
- REST API
- Webhooks
---
