---
api_key_in:
- header
api_specs:
- filename: amberflo-customers-api-openapi.yml
  format: yaml
  label: Amberflo Customers API
  slug: amberflo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-customers-api-openapi.yml
- filename: amberflo-event-ingestion-api-openapi.yml
  format: yaml
  label: Amberflo Event Ingestion API
  slug: amberflo-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-event-ingestion-api-openapi.yml
- filename: amberflo-filtering-rules-api-openapi.yml
  format: yaml
  label: Amberflo Filtering Rules API
  slug: amberflo-filtering-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-filtering-rules-api-openapi.yml
- filename: amberflo-invoices-api-openapi.yml
  format: yaml
  label: Amberflo Invoices API
  slug: amberflo-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-invoices-api-openapi.yml
- filename: amberflo-meter-definitions-api-openapi.yml
  format: yaml
  label: Amberflo Meter Definitions API
  slug: amberflo-meter-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-meter-definitions-api-openapi.yml
- filename: amberflo-prepaid-orders-api-openapi.yml
  format: yaml
  label: Amberflo Prepaid Orders API
  slug: amberflo-prepaid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-prepaid-orders-api-openapi.yml
- filename: amberflo-pricing-plans-api-openapi.yml
  format: yaml
  label: Amberflo Pricing Plans API
  slug: amberflo-pricing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-pricing-plans-api-openapi.yml
- filename: amberflo-usage-queries-api-openapi.yml
  format: yaml
  label: Amberflo Usage Queries API
  slug: amberflo-usage-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/openapi/amberflo-usage-queries-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amberflo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amberflo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amberflo
provider_slug: amberflo
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/amberflo-billing-openapi.yaml
  - openapi/amberflo-metering-openapi.yaml
  type: apiKey
slug: amberflo-authentication
source_filename: amberflo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amberflo-billing-openapi.yaml, openapi/amberflo-metering-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication\n  sources:\n  - openapi/amberflo-billing-openapi.yaml\n  - openapi/amberflo-metering-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/authentication/amberflo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
---
