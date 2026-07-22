---
api_key_in:
- header
api_specs:
- filename: spektr-openapi.yml
  format: yaml
  label: Spektr API
  slug: spektr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spektr/refs/heads/main/openapi/spektr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spektr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spektr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spektr
provider_slug: spektr
scheme_count: 1
schemes:
- description: You can generate API keys in settings from the developer dashboard.
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/spektr-openapi.yml
  type: apiKey
slug: spektr-authentication
source_filename: spektr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spektr-openapi.yml\ndocs: https://spektr.readme.io/reference/welcome-to-spektr-api-documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Spektr uses a single API-key scheme. Keys are generated in the developer\n  dashboard (Settings) and sent on every request in the x-api-key header.\n  Keys are workspace-scoped. Webhook deliveries are separately authenticated\n  with an HMAC secret (see conventions/ and asyncapi/).\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: You can generate API keys in settings from the developer dashboard.\n  sources:\n  - openapi/spektr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spektr/refs/heads/main/authentication/spektr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- RegTech
- KYB
- KYC
- Onboarding
- Transaction Monitoring
- Financial Services
- Artificial Intelligence
- Enterprise
---
