---
api_key_in: []
api_specs:
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Work Orders API
  slug: shopmonkey-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Customers API
  slug: shopmonkey-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Vehicles API
  slug: shopmonkey-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Inventory & Parts API
  slug: shopmonkey-inventory-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Invoices & Payments API
  slug: shopmonkey-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Appointments API
  slug: shopmonkey-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Employees API
  slug: shopmonkey-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Locations API
  slug: shopmonkey-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Webhooks API
  slug: shopmonkey-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shopmonkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shopmonkey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shopmonkey
provider_slug: shopmonkey
scheme_count: 1
schemes:
- description: 'API key generated in the Shopmonkey web app under Settings > Integration > API Keys, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shopmonkey-openapi.yml
  type: http
slug: shopmonkey-authentication
source_filename: shopmonkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopmonkey-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key generated in the Shopmonkey web app under Settings > Integration > API\n    Keys, sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/shopmonkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/authentication/shopmonkey-authentication.yml
summary_line: http · 1 scheme
tags:
- Auto Repair
- Shop Management
- Field Service
- REST
- Not GraphQL
---
