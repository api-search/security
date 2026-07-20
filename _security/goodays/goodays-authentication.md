---
api_key_in:
- header
api_specs:
- filename: goodays-openapi-original.json
  format: json
  label: Goodays API
  slug: goodays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Goodays Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodays secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Goodays
provider_slug: goodays
scheme_count: 1
schemes:
- description: Personal access token supplied verbatim in the Authorization header (no Bearer prefix). Obtain from your Goodays account manager.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/goodays-openapi-original.json
  type: apiKey
slug: goodays-authentication
source_filename: goodays-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/goodays-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Personal access token supplied verbatim in the Authorization header (no Bearer\n    prefix). Obtain from your Goodays account manager.\n  sources:\n  - openapi/goodays-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/authentication/goodays-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Experience
- Customer Feedback
- Voice of the Customer
- Surveys
- NPS
- Reviews
- Retail
- CRM
- SaaS
---
