---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gingr-invoices-api-openapi.yml
  format: yaml
  label: Gingr Invoices API
  slug: gingr-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-invoices-api-openapi.yml
- filename: gingr-payments-api-openapi.yml
  format: yaml
  label: Gingr Payments API
  slug: gingr-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payments-api-openapi.yml
- filename: gingr-pets-api-openapi.yml
  format: yaml
  label: Gingr Pets API
  slug: gingr-pets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-pets-api-openapi.yml
- filename: gingr-booking-type-rates-api-openapi.yml
  format: yaml
  label: Gingr Booking Type Rates API
  slug: gingr-booking-type-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-booking-type-rates-api-openapi.yml
- filename: gingr-bookings-api-openapi.yml
  format: yaml
  label: Gingr Bookings API
  slug: gingr-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-bookings-api-openapi.yml
- filename: gingr-card-on-file-api-openapi.yml
  format: yaml
  label: Gingr Card On File API
  slug: gingr-card-on-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-card-on-file-api-openapi.yml
- filename: gingr-config-api-openapi.yml
  format: yaml
  label: Gingr Config API
  slug: gingr-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-config-api-openapi.yml
- filename: gingr-group-classes-api-openapi.yml
  format: yaml
  label: Gingr Group Classes API
  slug: gingr-group-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-group-classes-api-openapi.yml
- filename: gingr-parents-api-openapi.yml
  format: yaml
  label: Gingr Parents API
  slug: gingr-parents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-parents-api-openapi.yml
- filename: gingr-payment-api-openapi.yml
  format: yaml
  label: Gingr Payment API
  slug: gingr-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payment-api-openapi.yml
- filename: gingr-precheck-api-openapi.yml
  format: yaml
  label: Gingr Precheck API
  slug: gingr-precheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-precheck-api-openapi.yml
- filename: gingr-upload-api-openapi.yml
  format: yaml
  label: Gingr Upload API
  slug: gingr-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-upload-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gingr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gingr secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gingr
provider_slug: gingr
scheme_count: 1
schemes:
- description: 'API key issued per Gingr account from the "Manage Account" > API area of the Gingr console. Every request additionally requires a `subdomain` header identifying the Gingr account, and an `Accept: application/vnd.api+json` header.'
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/gingr-openapi.yml
  type: apiKey
slug: gingr-authentication
source_filename: gingr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gingr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'API key issued per Gingr account from the \"Manage Account\" > API area of the\n    Gingr console. Every request additionally requires a `subdomain` header identifying the\n    Gingr account, and an `Accept: application/vnd.api+json` header.'\n  sources:\n  - openapi/gingr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gingr/authentication/gingr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pet Care
- Pet Daycare
- Boarding
- Grooming
- Vertical SaaS
- Scheduling
- Payments
---
