---
api_key_in:
- header
api_specs:
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Orders API
  slug: ezrentout-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Fixed Assets API
  slug: ezrentout-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Inventory API
  slug: ezrentout-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Bundles API
  slug: ezrentout-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Customers API
  slug: ezrentout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Members API
  slug: ezrentout-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Locations API
  slug: ezrentout-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Availability API
  slug: ezrentout-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Payments and Invoicing API
  slug: ezrentout-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Purchase Orders API
  slug: ezrentout-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
- filename: ezrentout-openapi.yml
  format: yaml
  label: EZRentOut Maintenance and Work Orders API
  slug: ezrentout-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/openapi/ezrentout-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ezrentout Authentication
name_suffix: Authentication
oauth_flows: []
overview: EZRentOut secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EZRentOut
provider_slug: ezrentout
scheme_count: 1
schemes:
- description: Per-company access token generated in Settings (API must be enabled by the account owner). Sent in the `token` HTTP header on every request over HTTPS.
  in: header
  name: tokenAuth
  parameter: token
  sources:
  - openapi/ezrentout-openapi.yml
  type: apiKey
slug: ezrentout-authentication
source_filename: ezrentout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ezrentout-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: token\n  description: Per-company access token generated in Settings (API must be enabled by the account\n    owner). Sent in the `token` HTTP header on every request over HTTPS.\n  sources:\n  - openapi/ezrentout-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezrentout/refs/heads/main/authentication/ezrentout-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Equipment Rental
- Rental Management
- Asset Tracking
- Inventory
- Order Management
- EZO
---
