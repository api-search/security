---
api_key_in: []
api_specs:
- filename: fastspring-accounts-api-openapi.yml
  format: yaml
  label: FastSpring Accounts API
  slug: fastspring-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-accounts-api-openapi.yml
- filename: fastspring-coupons-api-openapi.yml
  format: yaml
  label: FastSpring Coupons API
  slug: fastspring-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-coupons-api-openapi.yml
- filename: fastspring-data-api-openapi.yml
  format: yaml
  label: FastSpring Data API
  slug: fastspring-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-data-api-openapi.yml
- filename: fastspring-events-api-openapi.yml
  format: yaml
  label: FastSpring Events API
  slug: fastspring-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-events-api-openapi.yml
- filename: fastspring-invoices-api-openapi.yml
  format: yaml
  label: FastSpring Invoices API
  slug: fastspring-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-invoices-api-openapi.yml
- filename: fastspring-orders-api-openapi.yml
  format: yaml
  label: FastSpring Orders API
  slug: fastspring-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-orders-api-openapi.yml
- filename: fastspring-products-api-openapi.yml
  format: yaml
  label: FastSpring Products API
  slug: fastspring-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-products-api-openapi.yml
- filename: fastspring-quotes-api-openapi.yml
  format: yaml
  label: FastSpring Quotes API
  slug: fastspring-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-quotes-api-openapi.yml
- filename: fastspring-returns-api-openapi.yml
  format: yaml
  label: FastSpring Returns API
  slug: fastspring-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-returns-api-openapi.yml
- filename: fastspring-sessions-api-openapi.yml
  format: yaml
  label: FastSpring Sessions API
  slug: fastspring-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-sessions-api-openapi.yml
- filename: fastspring-subscriptions-api-openapi.yml
  format: yaml
  label: FastSpring Subscriptions API
  slug: fastspring-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-subscriptions-api-openapi.yml
- filename: fastspring-webhooks-api-openapi.yml
  format: yaml
  label: FastSpring Webhooks API
  slug: fastspring-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fastspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastSpring secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FastSpring
provider_slug: fastspring
scheme_count: 1
schemes:
- description: HTTP Basic with credentials from FastSpring App Dashboard
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/fastspring-openapi.yml
  type: http
slug: fastspring-authentication
source_filename: fastspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fastspring-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with credentials from FastSpring App Dashboard\n  sources:\n  - openapi/fastspring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/authentication/fastspring-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Merchant of Record
- Subscription Billing
- Payments
- SaaS Billing
- Checkout
- Tax Compliance
---
