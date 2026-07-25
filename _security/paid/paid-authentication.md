---
api_key_in: []
api_specs:
- filename: paid-agents-api-openapi.yml
  format: yaml
  label: Paid agents API
  slug: paid-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-agents-api-openapi.yml
- filename: paid-analyticsexperimental-api-openapi.yml
  format: yaml
  label: Paid analyticsExperimental API
  slug: paid-analyticsexperimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-analyticsexperimental-api-openapi.yml
- filename: paid-checkouts-api-openapi.yml
  format: yaml
  label: Paid checkouts API
  slug: paid-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-checkouts-api-openapi.yml
- filename: paid-contacts-api-openapi.yml
  format: yaml
  label: Paid contacts API
  slug: paid-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-contacts-api-openapi.yml
- filename: paid-costs-api-openapi.yml
  format: yaml
  label: Paid costs API
  slug: paid-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-costs-api-openapi.yml
- filename: paid-credits-api-openapi.yml
  format: yaml
  label: Paid credits API
  slug: paid-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-credits-api-openapi.yml
- filename: paid-customer-groups-api-openapi.yml
  format: yaml
  label: Paid customer-groups API
  slug: paid-customer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-customer-groups-api-openapi.yml
- filename: paid-customer-portals-api-openapi.yml
  format: yaml
  label: Paid customer-portals API
  slug: paid-customer-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-customer-portals-api-openapi.yml
- filename: paid-customers-api-openapi.yml
  format: yaml
  label: Paid customers API
  slug: paid-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-customers-api-openapi.yml
- filename: paid-customviewsexperimental-api-openapi.yml
  format: yaml
  label: Paid customViewsExperimental API
  slug: paid-customviewsexperimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-customviewsexperimental-api-openapi.yml
- filename: paid-invoices-api-openapi.yml
  format: yaml
  label: Paid invoices API
  slug: paid-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-invoices-api-openapi.yml
- filename: paid-orders-api-openapi.yml
  format: yaml
  label: Paid orders API
  slug: paid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-orders-api-openapi.yml
- filename: paid-orders-lines-api-openapi.yml
  format: yaml
  label: Paid orders > lines API
  slug: paid-orders-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-orders-lines-api-openapi.yml
- filename: paid-plans-api-openapi.yml
  format: yaml
  label: Paid plans API
  slug: paid-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-plans-api-openapi.yml
- filename: paid-pricing-api-openapi.yml
  format: yaml
  label: Paid pricing API
  slug: paid-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-pricing-api-openapi.yml
- filename: paid-products-api-openapi.yml
  format: yaml
  label: Paid products API
  slug: paid-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-products-api-openapi.yml
- filename: paid-signals-api-openapi.yml
  format: yaml
  label: Paid signals API
  slug: paid-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-signals-api-openapi.yml
- filename: paid-traces-api-openapi.yml
  format: yaml
  label: Paid traces API
  slug: paid-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-traces-api-openapi.yml
- filename: paid-usage-api-openapi.yml
  format: yaml
  label: Paid usage API
  slug: paid-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-usage-api-openapi.yml
- filename: paid-value-models-api-openapi.yml
  format: yaml
  label: Paid value-models API
  slug: paid-value-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-value-models-api-openapi.yml
- filename: paid-value-receipts-api-openapi.yml
  format: yaml
  label: Paid value-receipts API
  slug: paid-value-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-value-receipts-api-openapi.yml
- filename: paid-webhooks-api-openapi.yml
  format: yaml
  label: Paid webhooks API
  slug: paid-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Paid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paid
provider_slug: paid
scheme_count: 1
schemes:
- description: API key authentication using a Bearer token. Keys are prefixed `paid_` and issued from the Paid app.
  header: 'Authorization: Bearer paid_xxx'
  issued_at: https://app.paid.ai/settings/api-keys
  key_prefix: paid_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paid-v1.json
  - openapi/paid-v2.json
  type: http
slug: paid-authentication
source_filename: paid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paid-v1.json, openapi/paid-v2.json, https://docs.paid.ai/documentation/getting-started/quickstart\ndocs: https://docs.paid.ai/cli/cli/command-reference\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication using a Bearer token. Keys are prefixed `paid_`\n    and issued from the Paid app.\n  key_prefix: paid_\n  header: 'Authorization: Bearer paid_xxx'\n  issued_at: https://app.paid.ai/settings/api-keys\n  sources:\n  - openapi/paid-v1.json\n  - openapi/paid-v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/authentication/paid-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Billing
- Monetization
- Payments
- Usage-Based Pricing
- AI Agents
- FinOps
---
