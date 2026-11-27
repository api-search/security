---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: midax402-com-badge-api-openapi.yml
  format: yaml
  label: MIDAX402 Badge API
  slug: midax402-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midax402-com/openapi/midax402-com-badge-api-openapi.yml
- filename: midax402-com-midas-ops-api-openapi.yml
  format: yaml
  label: MIDAX402 Midas Ops API
  slug: midax402-com-midas-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midax402-com/openapi/midax402-com-midas-ops-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MIDAX402 Authentication
name_suffix: Authentication
oauth_flows: []
overview: MIDAX402 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MIDAX402
provider_slug: midax402-com
scheme_count: 1
schemes:
- description: x402 payment proof header. Clients may also send X-PAYMENT depending on their SDK.
  in: header
  name: x402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/midax402-com-openapi.json
  type: apiKey
slug: midax402-com-authentication
source_filename: midax402-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/midax402-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 payment proof header. Clients may also send X-PAYMENT depending on their\n    SDK.\n  sources:\n  - openapi/midax402-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/midax402-com/authentication/midax402-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Verification
- x402
- Data Intelligence
---
