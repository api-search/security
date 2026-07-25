---
api_key_in: []
api_specs:
- filename: chartmogul-asyncapi.yml
  format: yaml
  label: ChartMogul Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-asyncapi.yml
- filename: chartmogul-account-api-openapi.yml
  format: yaml
  label: ChartMogul Account API
  slug: chartmogul-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-account-api-openapi.yml
- filename: chartmogul-customers-api-openapi.yml
  format: yaml
  label: ChartMogul Customers API
  slug: chartmogul-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-customers-api-openapi.yml
- filename: chartmogul-invoices-api-openapi.yml
  format: yaml
  label: ChartMogul Invoices API
  slug: chartmogul-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-invoices-api-openapi.yml
- filename: chartmogul-metrics-api-openapi.yml
  format: yaml
  label: ChartMogul Metrics API
  slug: chartmogul-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-metrics-api-openapi.yml
- filename: chartmogul-plans-api-openapi.yml
  format: yaml
  label: ChartMogul Plans API
  slug: chartmogul-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-plans-api-openapi.yml
- filename: chartmogul-subscriptions-api-openapi.yml
  format: yaml
  label: ChartMogul Subscriptions API
  slug: chartmogul-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/openapi/chartmogul-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chartmogul Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChartMogul secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChartMogul
provider_slug: chartmogul
scheme_count: 1
schemes:
- description: HTTP Basic Auth. Username is your ChartMogul API key; password is empty.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/chartmogul-openapi.yml
  type: http
slug: chartmogul-authentication
source_filename: chartmogul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chartmogul-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth. Username is your ChartMogul API key; password is empty.\n  sources:\n  - openapi/chartmogul-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartmogul/refs/heads/main/authentication/chartmogul-authentication.yml
summary_line: http · 1 scheme
tags:
- Subscription Analytics
- SaaS Metrics
- Revenue Analytics
- MRR
- Churn
- Cohorts
- Billing
---
