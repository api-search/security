---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Baremetrics API
  slug: baremetrics-api
  spec_type: OpenAPI
  url: https://developers.baremetrics.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Baremetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baremetrics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Baremetrics
provider_slug: baremetrics
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/baremetrics-openapi.json
  type: apiKey
slug: baremetrics-authentication
source_filename: baremetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/baremetrics-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/baremetrics-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/authentication/baremetrics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscription Analytics
- MRR
- ARR
- Churn Rate
- LTV
- Revenue
- Stripe
- Financial Metrics
- SaaS
---
