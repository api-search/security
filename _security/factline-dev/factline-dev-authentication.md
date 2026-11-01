---
anonymous_access: false
api_key_in: []
api_specs:
- filename: factline-dev-free-api-openapi.yml
  format: yaml
  label: factline-dev Free API
  slug: factline-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factline-dev/openapi/factline-dev-free-api-openapi.yml
- filename: factline-dev-paid-x402-api-openapi.yml
  format: yaml
  label: factline-dev Paid (x402) API
  slug: factline-dev-paid-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factline-dev/openapi/factline-dev-paid-x402-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Factline Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: factline-dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: factline-dev
provider_slug: factline-dev
scheme_count: 1
schemes:
- description: Optional business API key (fl_live_...), billed monthly instead of per call. See https://factline.dev/business
  name: apiKey
  scheme: bearer
  sources:
  - openapi/factline-dev-openapi.json
  type: http
slug: factline-dev-authentication
source_filename: factline-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/factline-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Optional business API key (fl_live_...), billed monthly instead of per call.\n    See https://factline.dev/business\n  sources:\n  - openapi/factline-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/factline-dev/authentication/factline-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Compliance
- KYB
- API
---
