---
api_key_in: []
api_specs:
- filename: loop-openapi-original.json
  format: json
  label: Loop API
  slug: loop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-openapi-original.json
- filename: loop-onboarding-openapi-original.json
  format: json
  label: Loop Onboarding API
  slug: loop-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-onboarding-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Loop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loop
provider_slug: loop
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: "Bearer HTTP authentication. Allowed headers: \n  Authorization: Bearer <apiKey>"
  name: bearer
  scheme: bearer
  sources:
  - openapi/loop-onboarding-openapi-original.json
  - openapi/loop-openapi-original.json
  type: http
slug: loop-authentication
source_filename: loop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/loop-onboarding-openapi-original.json, openapi/loop-openapi-original.json\ndocs: https://docs.loop.com/developers/api-authentication\ndetail:\n  model: Bearer API key\n  header: 'Authorization: Bearer <apiKey>'\n  key_prefix: lk_live_\n  provisioning: API keys are issued by your Loop contact (no self-service token endpoint).\n  validation_endpoint: GET /v1/ping (HTTP 200 on a valid key)\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: \"Bearer HTTP authentication. Allowed headers: \\n  Authorization: Bearer <apiKey>\"\n  sources:\n  - openapi/loop-onboarding-openapi-original.json\n  - openapi/loop-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/authentication/loop-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Supply Chain
- Freight
- Freight Audit
- Payments
- Transportation
- Artificial Intelligence
- Data Platform
---
