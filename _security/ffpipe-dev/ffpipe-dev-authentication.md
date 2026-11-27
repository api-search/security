---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ffpipe-dev-discovery-api-openapi.yml
  format: yaml
  label: ffpipe Discovery API
  slug: ffpipe-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-discovery-api-openapi.yml
- filename: ffpipe-dev-feedback-api-openapi.yml
  format: yaml
  label: ffpipe Feedback API
  slug: ffpipe-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-feedback-api-openapi.yml
- filename: ffpipe-dev-jobs-api-openapi.yml
  format: yaml
  label: ffpipe Jobs API
  slug: ffpipe-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-jobs-api-openapi.yml
- filename: ffpipe-dev-mcp-api-openapi.yml
  format: yaml
  label: ffpipe MCP API
  slug: ffpipe-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffpipe-dev/openapi/ffpipe-dev-mcp-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: ffpipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: ffpipe secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ffpipe
provider_slug: ffpipe-dev
scheme_count: 2
schemes:
- description: 'Not an API key: an x402 v2 payment payload, freshly signed per request from the PAYMENT-REQUIRED challenge. Modelled as apiKey because OpenAPI has no x402 security type — see the `x-x402` extensions.'
  in: header
  name: x402
  parameter: payment-signature
  sources:
  - openapi/ffpipe-dev-openapi.json
  type: apiKey
- description: Single-use retry credential issued when a paid job failed on our side.
  in: header
  name: retryVoucher
  parameter: x-retry-voucher
  sources:
  - openapi/ffpipe-dev-openapi.json
  type: apiKey
slug: ffpipe-dev-authentication
source_filename: ffpipe-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/ffpipe-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: apiKey\n  in: header\n  parameter: payment-signature\n  description: 'Not an API key: an x402 v2 payment payload, freshly signed per request from\n    the PAYMENT-REQUIRED challenge. Modelled as apiKey because OpenAPI has no x402 security\n    type — see the `x-x402` extensions.'\n  sources:\n  - openapi/ffpipe-dev-openapi.json\n- name: retryVoucher\n  type: apiKey\n  in: header\n  parameter: x-retry-voucher\n  description: Single-use retry credential issued when a paid job failed on our side.\n  sources:\n  - openapi/ffpipe-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ffpipe-dev/authentication/ffpipe-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Media
- Payments
- Video
- Automation
---
