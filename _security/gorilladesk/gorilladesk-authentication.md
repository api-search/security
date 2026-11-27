---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gorilladesk-company-api-openapi.yml
  format: yaml
  label: GorillaDesk Company API
  slug: gorilladesk-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-company-api-openapi.yml
- filename: gorilladesk-customer-api-openapi.yml
  format: yaml
  label: GorillaDesk Customer API
  slug: gorilladesk-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-customer-api-openapi.yml
- filename: gorilladesk-note-api-openapi.yml
  format: yaml
  label: GorillaDesk Note API
  slug: gorilladesk-note-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-note-api-openapi.yml
- filename: gorilladesk-phone-type-api-openapi.yml
  format: yaml
  label: GorillaDesk Phone Type API
  slug: gorilladesk-phone-type-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-phone-type-api-openapi.yml
- filename: gorilladesk-user-api-openapi.yml
  format: yaml
  label: GorillaDesk User API
  slug: gorilladesk-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-user-api-openapi.yml
- filename: gorilladesk-branches-api-openapi.yml
  format: yaml
  label: GorillaDesk Branches API
  slug: gorilladesk-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-branches-api-openapi.yml
- filename: gorilladesk-credits-api-openapi.yml
  format: yaml
  label: GorillaDesk Credits API
  slug: gorilladesk-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-credits-api-openapi.yml
- filename: gorilladesk-customers-api-openapi.yml
  format: yaml
  label: GorillaDesk Customers API
  slug: gorilladesk-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-customers-api-openapi.yml
- filename: gorilladesk-documents-api-openapi.yml
  format: yaml
  label: GorillaDesk Documents API
  slug: gorilladesk-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-documents-api-openapi.yml
- filename: gorilladesk-estimates-api-openapi.yml
  format: yaml
  label: GorillaDesk Estimates API
  slug: gorilladesk-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-estimates-api-openapi.yml
- filename: gorilladesk-invoices-api-openapi.yml
  format: yaml
  label: GorillaDesk Invoices API
  slug: gorilladesk-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-invoices-api-openapi.yml
- filename: gorilladesk-jobs-api-openapi.yml
  format: yaml
  label: GorillaDesk Jobs API
  slug: gorilladesk-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-jobs-api-openapi.yml
- filename: gorilladesk-line-items-api-openapi.yml
  format: yaml
  label: GorillaDesk Line Items API
  slug: gorilladesk-line-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-line-items-api-openapi.yml
- filename: gorilladesk-payment-methods-api-openapi.yml
  format: yaml
  label: GorillaDesk Payment Methods API
  slug: gorilladesk-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-payment-methods-api-openapi.yml
- filename: gorilladesk-payments-api-openapi.yml
  format: yaml
  label: GorillaDesk Payments API
  slug: gorilladesk-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-payments-api-openapi.yml
- filename: gorilladesk-recurring-invoices-api-openapi.yml
  format: yaml
  label: GorillaDesk Recurring Invoices API
  slug: gorilladesk-recurring-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-recurring-invoices-api-openapi.yml
- filename: gorilladesk-schedules-api-openapi.yml
  format: yaml
  label: GorillaDesk Schedules API
  slug: gorilladesk-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-schedules-api-openapi.yml
- filename: gorilladesk-service-templates-api-openapi.yml
  format: yaml
  label: GorillaDesk Service Templates API
  slug: gorilladesk-service-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-service-templates-api-openapi.yml
- filename: gorilladesk-sources-api-openapi.yml
  format: yaml
  label: GorillaDesk Sources API
  slug: gorilladesk-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-sources-api-openapi.yml
- filename: gorilladesk-taxes-api-openapi.yml
  format: yaml
  label: GorillaDesk Taxes API
  slug: gorilladesk-taxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gorilladesk/openapi/gorilladesk-taxes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GorillaDesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: GorillaDesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GorillaDesk
provider_slug: gorilladesk
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/gorilladesk-openapi.yml
  type: http
slug: gorilladesk-authentication
source_filename: gorilladesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gorilladesk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gorilladesk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gorilladesk/authentication/gorilladesk-authentication.yml
summary_line: http · 1 scheme
tags:
- Field Service Management
- Pest Control
- Lawn Care
- Scheduling
- Invoicing
- Customers
- Software-as-a-Service
---
