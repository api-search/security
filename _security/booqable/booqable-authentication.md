---
api_key_in: []
api_specs:
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Orders API
  slug: booqable-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Order Fulfillment API
  slug: booqable-order-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Products API
  slug: booqable-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Product Groups API
  slug: booqable-product-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Customers API
  slug: booqable-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Stock Items API
  slug: booqable-stock-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Availability API
  slug: booqable-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Documents & Invoices API
  slug: booqable-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Bundles & Collections API
  slug: booqable-bundles-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Webhooks API
  slug: booqable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Settings & Locations API
  slug: booqable-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Booqable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booqable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Booqable
provider_slug: booqable
scheme_count: 1
schemes:
- description: 'An access token created in Booqable account settings, sent as "Authorization: Bearer <token>". Booqable also supports request signing (single-use signed tokens using ES256, RS256, or HS256) and, on the legacy v1 API, an api_key query parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/booqable-openapi.yml
  type: http
slug: booqable-authentication
source_filename: booqable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/booqable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An access token created in Booqable account settings, sent as \"Authorization:\n    Bearer <token>\". Booqable also supports request signing (single-use signed tokens using\n    ES256, RS256, or HS256) and, on the legacy v1 API, an api_key query parameter.'\n  sources:\n  - openapi/booqable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/authentication/booqable-authentication.yml
summary_line: http · 1 scheme
tags:
- Rental Management
- Inventory
- Equipment Rental
- Bookings
- Orders
- E-commerce
- JSON:API
---
