---
api_key_in:
- header
api_specs:
- filename: benchmark-email-benchmark-email-api-openapi.yml
  format: yaml
  label: Benchmark Email RESTful API v3.0
  slug: benchmark-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchmark-email/refs/heads/main/openapi/benchmark-email-benchmark-email-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Benchmark Email Authentication
name_suffix: Authentication
oauth_flows: []
overview: Benchmark Email secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Benchmark Email
provider_slug: benchmark-email
scheme_count: 1
schemes:
- description: API token obtained from https://ui.benchmarkemail.com/Integrate#API
  in: header
  name: apiKeyAuth
  parameter: AuthToken
  sources:
  - openapi/benchmark-email-benchmark-email-api-openapi.yml
  type: apiKey
slug: benchmark-email-authentication
source_filename: benchmark-email-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benchmark-email-benchmark-email-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: AuthToken\n  description: API token obtained from https://ui.benchmarkemail.com/Integrate#API\n  sources:\n  - openapi/benchmark-email-benchmark-email-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmark-email/refs/heads/main/authentication/benchmark-email-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Marketing
- Campaigns
- Contacts
- Automation
- Transactional Email
- Marketing
---
