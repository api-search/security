---
api_key_in: []
api_specs:
- filename: paddle-addresses-api-openapi.yml
  format: yaml
  label: Paddle Addresses API
  slug: paddle-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-addresses-api-openapi.yml
- filename: paddle-adjustments-api-openapi.yml
  format: yaml
  label: Paddle Adjustments API
  slug: paddle-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-adjustments-api-openapi.yml
- filename: paddle-businesses-api-openapi.yml
  format: yaml
  label: Paddle Businesses API
  slug: paddle-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-businesses-api-openapi.yml
- filename: paddle-customers-api-openapi.yml
  format: yaml
  label: Paddle Customers API
  slug: paddle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-customers-api-openapi.yml
- filename: paddle-discounts-api-openapi.yml
  format: yaml
  label: Paddle Discounts API
  slug: paddle-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-discounts-api-openapi.yml
- filename: paddle-event-types-api-openapi.yml
  format: yaml
  label: Paddle Event Types API
  slug: paddle-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-event-types-api-openapi.yml
- filename: paddle-events-api-openapi.yml
  format: yaml
  label: Paddle Events API
  slug: paddle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-events-api-openapi.yml
- filename: paddle-notification-settings-api-openapi.yml
  format: yaml
  label: Paddle Notification Settings API
  slug: paddle-notification-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-notification-settings-api-openapi.yml
- filename: paddle-notifications-api-openapi.yml
  format: yaml
  label: Paddle Notifications API
  slug: paddle-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-notifications-api-openapi.yml
- filename: paddle-prices-api-openapi.yml
  format: yaml
  label: Paddle Prices API
  slug: paddle-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-prices-api-openapi.yml
- filename: paddle-products-api-openapi.yml
  format: yaml
  label: Paddle Products API
  slug: paddle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-products-api-openapi.yml
- filename: paddle-reports-api-openapi.yml
  format: yaml
  label: Paddle Reports API
  slug: paddle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-reports-api-openapi.yml
- filename: paddle-subscriptions-api-openapi.yml
  format: yaml
  label: Paddle Subscriptions API
  slug: paddle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-subscriptions-api-openapi.yml
- filename: paddle-transactions-api-openapi.yml
  format: yaml
  label: Paddle Transactions API
  slug: paddle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paddle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paddle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paddle
provider_slug: paddle
scheme_count: 1
schemes:
- description: 'Authenticate with your Paddle API key passed in the Authorization header with the Bearer prefix, e.g. `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paddle-openapi.yml
  type: http
slug: paddle-authentication
source_filename: paddle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paddle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with your Paddle API key passed in the Authorization header with\n    the Bearer prefix, e.g. `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/paddle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/authentication/paddle-authentication.yml
summary_line: http · 1 scheme
tags:
- Billing
- Payments
- Subscription
- Merchant of Record
- Software-as-a-Service
---
