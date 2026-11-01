---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: skavio-eu-batch-processing-api-openapi.yml
  format: yaml
  label: skavio-eu Batch processing API
  slug: skavio-eu-batch-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-batch-processing-api-openapi.yml
- filename: skavio-eu-billing-api-openapi.yml
  format: yaml
  label: skavio-eu Billing API
  slug: skavio-eu-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-billing-api-openapi.yml
- filename: skavio-eu-bulk-manifests-api-openapi.yml
  format: yaml
  label: skavio-eu Bulk manifests API
  slug: skavio-eu-bulk-manifests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-bulk-manifests-api-openapi.yml
- filename: skavio-eu-contacts-api-openapi.yml
  format: yaml
  label: skavio-eu Contacts API
  slug: skavio-eu-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-contacts-api-openapi.yml
- filename: skavio-eu-events-api-openapi.yml
  format: yaml
  label: skavio-eu Events API
  slug: skavio-eu-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-events-api-openapi.yml
- filename: skavio-eu-flow-api-openapi.yml
  format: yaml
  label: skavio-eu Flow API
  slug: skavio-eu-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-flow-api-openapi.yml
- filename: skavio-eu-invoices-api-openapi.yml
  format: yaml
  label: skavio-eu Invoices API
  slug: skavio-eu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-invoices-api-openapi.yml
- filename: skavio-eu-me-api-openapi.yml
  format: yaml
  label: skavio-eu Me API
  slug: skavio-eu-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-me-api-openapi.yml
- filename: skavio-eu-operational-notifications-api-openapi.yml
  format: yaml
  label: skavio-eu Operational notifications API
  slug: skavio-eu-operational-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-operational-notifications-api-openapi.yml
- filename: skavio-eu-paid-web-data-api-openapi.yml
  format: yaml
  label: skavio-eu paid web data API
  slug: skavio-eu-paid-web-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-paid-web-data-api-openapi.yml
- filename: skavio-eu-requests-api-openapi.yml
  format: yaml
  label: skavio-eu Requests API
  slug: skavio-eu-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-requests-api-openapi.yml
- filename: skavio-eu-skavio-accounting-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio Accounting API
  slug: skavio-eu-skavio-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-accounting-api-openapi.yml
- filename: skavio-eu-skavio-processing-api-api-openapi.yml
  format: yaml
  label: skavio-eu Skavio processing API
  slug: skavio-eu-skavio-processing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-skavio-processing-api-api-openapi.yml
- filename: skavio-eu-usdc-payment-verification-api-openapi.yml
  format: yaml
  label: skavio-eu USDC payment verification API
  slug: skavio-eu-usdc-payment-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-usdc-payment-verification-api-openapi.yml
- filename: skavio-eu-webhooks-api-openapi.yml
  format: yaml
  label: skavio-eu Webhooks API
  slug: skavio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-webhooks-api-openapi.yml
- filename: skavio-eu-workflow-pipelines-api-openapi.yml
  format: yaml
  label: skavio-eu Workflow pipelines API
  slug: skavio-eu-workflow-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-workflow-pipelines-api-openapi.yml
- filename: skavio-eu-x402-api-openapi.yml
  format: yaml
  label: skavio-eu X402 API
  slug: skavio-eu-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skavio-eu/openapi/skavio-eu-x402-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Skavio Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: skavio-eu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: skavio-eu
provider_slug: skavio-eu
scheme_count: 2
schemes:
- description: Company key created in the dashboard; read/write scopes.
  name: BearerKey
  scheme: bearer
  sources:
  - openapi/skavio-eu-processing-openapi.json
  - openapi/skavio-eu-proof-openapi.json
  type: http
- description: Interactive same-origin company session for administrative operations.
  in: cookie
  name: WebSession
  parameter: skavio_web_account
  sources:
  - openapi/skavio-eu-processing-openapi.json
  type: apiKey
slug: skavio-eu-authentication
source_filename: skavio-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/skavio-eu-processing-openapi.json, openapi/skavio-eu-proof-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: Company key created in the dashboard; read/write scopes.\n  sources:\n  - openapi/skavio-eu-processing-openapi.json\n  - openapi/skavio-eu-proof-openapi.json\n- name: WebSession\n  type: apiKey\n  in: cookie\n  parameter: skavio_web_account\n  description: Interactive same-origin company session for administrative operations.\n  sources:\n  - openapi/skavio-eu-processing-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/skavio-eu/authentication/skavio-eu-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- BusinessTools
- Document Processing
- Invoice Automation
- Audio Transcription
- Payments
---
