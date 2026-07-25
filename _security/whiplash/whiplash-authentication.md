---
api_key_in: []
api_specs:
- filename: whiplash-bundle-items-api-openapi.yml
  format: yaml
  label: Whiplash Bundle Items API
  slug: whiplash-bundle-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-bundle-items-api-openapi.yml
- filename: whiplash-consumer-returns-api-openapi.yml
  format: yaml
  label: Whiplash Consumer Returns API
  slug: whiplash-consumer-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-consumer-returns-api-openapi.yml
- filename: whiplash-customers-api-openapi.yml
  format: yaml
  label: Whiplash Customers API
  slug: whiplash-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-customers-api-openapi.yml
- filename: whiplash-documents-api-openapi.yml
  format: yaml
  label: Whiplash Documents API
  slug: whiplash-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-documents-api-openapi.yml
- filename: whiplash-items-api-openapi.yml
  format: yaml
  label: Whiplash Items API
  slug: whiplash-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-items-api-openapi.yml
- filename: whiplash-notification-events-api-openapi.yml
  format: yaml
  label: Whiplash Notification Events API
  slug: whiplash-notification-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-notification-events-api-openapi.yml
- filename: whiplash-notification-subscriptions-api-openapi.yml
  format: yaml
  label: Whiplash Notification Subscriptions API
  slug: whiplash-notification-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-notification-subscriptions-api-openapi.yml
- filename: whiplash-orders-api-openapi.yml
  format: yaml
  label: Whiplash Orders API
  slug: whiplash-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-orders-api-openapi.yml
- filename: whiplash-shipnotices-api-openapi.yml
  format: yaml
  label: Whiplash Shipnotices API
  slug: whiplash-shipnotices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-shipnotices-api-openapi.yml
- filename: whiplash-simulate-api-openapi.yml
  format: yaml
  label: Whiplash Simulate API
  slug: whiplash-simulate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-simulate-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Whiplash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whiplash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whiplash
provider_slug: whiplash
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: OAuth 2.0 Bearer token. Obtain via authorization code or client credentials flow. See https://help.whiplash.com/hc/en-us/articles/360050870691-Authentication-for-the-V2-API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/whiplash-openapi.json
  type: http
slug: whiplash-authentication
source_filename: whiplash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whiplash-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: OAuth 2.0 Bearer token. Obtain via authorization code or client credentials flow.\n    See https://help.whiplash.com/hc/en-us/articles/360050870691-Authentication-for-the-V2-API\n  sources:\n  - openapi/whiplash-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/authentication/whiplash-authentication.yml
summary_line: http · 1 scheme
tags:
- Fulfillment
- 3PL
- Logistics
- Ecommerce
- Orders
- Inventory
- Shipments
- Returns
- Warehousing
---
