---
api_key_in: []
api_specs:
- filename: loop-artifacts-api-openapi.yml
  format: yaml
  label: Loop artifacts API
  slug: loop-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-artifacts-api-openapi.yml
- filename: loop-artifacts-schema-validated-api-openapi.yml
  format: yaml
  label: Loop artifacts-schema-validated API
  slug: loop-artifacts-schema-validated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-artifacts-schema-validated-api-openapi.yml
- filename: loop-business-exceptions-api-openapi.yml
  format: yaml
  label: Loop business-exceptions API
  slug: loop-business-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-business-exceptions-api-openapi.yml
- filename: loop-factoring-relationships-api-openapi.yml
  format: yaml
  label: Loop factoring-relationships API
  slug: loop-factoring-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-factoring-relationships-api-openapi.yml
- filename: loop-invoicing-relationships-api-openapi.yml
  format: yaml
  label: Loop invoicing-relationships API
  slug: loop-invoicing-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-invoicing-relationships-api-openapi.yml
- filename: loop-onboarding-api-loop-com-api-openapi.yml
  format: yaml
  label: Loop onboarding.api.loop.com API
  slug: loop-onboarding-api-loop-com-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-onboarding-api-loop-com-api-openapi.yml
- filename: loop-organizations-api-openapi.yml
  format: yaml
  label: Loop organizations API
  slug: loop-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-organizations-api-openapi.yml
- filename: loop-payable-allocations-api-openapi.yml
  format: yaml
  label: Loop payable-allocations API
  slug: loop-payable-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-payable-allocations-api-openapi.yml
- filename: loop-payable-invoice-reviews-api-openapi.yml
  format: yaml
  label: Loop payable-invoice-reviews API
  slug: loop-payable-invoice-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-payable-invoice-reviews-api-openapi.yml
- filename: loop-payable-invoices-api-openapi.yml
  format: yaml
  label: Loop payable-invoices API
  slug: loop-payable-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-payable-invoices-api-openapi.yml
- filename: loop-payments-api-openapi.yml
  format: yaml
  label: Loop payments API
  slug: loop-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-payments-api-openapi.yml
- filename: loop-ping-api-openapi.yml
  format: yaml
  label: Loop ping API
  slug: loop-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-ping-api-openapi.yml
- filename: loop-receivable-invoices-api-openapi.yml
  format: yaml
  label: Loop receivable-invoices API
  slug: loop-receivable-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-receivable-invoices-api-openapi.yml
- filename: loop-shipment-jobs-api-openapi.yml
  format: yaml
  label: Loop shipment-jobs API
  slug: loop-shipment-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-shipment-jobs-api-openapi.yml
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
