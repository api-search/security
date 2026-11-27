---
anonymous_access: false
api_key_in: []
api_specs:
- filename: officina-it-articles-api-openapi.yml
  format: yaml
  label: officina.it Articles API
  slug: officina-it-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-articles-api-openapi.yml
- filename: officina-it-authentication-api-openapi.yml
  format: yaml
  label: officina.it Authentication API
  slug: officina-it-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-authentication-api-openapi.yml
- filename: officina-it-calendar-api-openapi.yml
  format: yaml
  label: officina.it Calendar API
  slug: officina-it-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-calendar-api-openapi.yml
- filename: officina-it-cashbook-api-openapi.yml
  format: yaml
  label: officina.it Cash Book API
  slug: officina-it-cashbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-cashbook-api-openapi.yml
- filename: officina-it-cestino-api-openapi.yml
  format: yaml
  label: officina.it Cestino API
  slug: officina-it-cestino-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-cestino-api-openapi.yml
- filename: officina-it-creditnotes-api-openapi.yml
  format: yaml
  label: officina.it Credit Notes API
  slug: officina-it-creditnotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-creditnotes-api-openapi.yml
- filename: officina-it-customers-api-openapi.yml
  format: yaml
  label: officina.it Customers API
  slug: officina-it-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-customers-api-openapi.yml
- filename: officina-it-dealership-api-openapi.yml
  format: yaml
  label: officina.it Dealership API
  slug: officina-it-dealership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-dealership-api-openapi.yml
- filename: officina-it-electronicinvoicing-api-openapi.yml
  format: yaml
  label: officina.it Electronic Invoicing API
  slug: officina-it-electronicinvoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-electronicinvoicing-api-openapi.yml
- filename: officina-it-expenses-api-openapi.yml
  format: yaml
  label: officina.it Expenses API
  slug: officina-it-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-expenses-api-openapi.yml
- filename: officina-it-invoices-api-openapi.yml
  format: yaml
  label: officina.it Invoices API
  slug: officina-it-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-invoices-api-openapi.yml
- filename: officina-it-quotes-api-openapi.yml
  format: yaml
  label: officina.it Quotes API
  slug: officina-it-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-quotes-api-openapi.yml
- filename: officina-it-receipts-api-openapi.yml
  format: yaml
  label: officina.it Receipts API
  slug: officina-it-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-receipts-api-openapi.yml
- filename: officina-it-reports-api-openapi.yml
  format: yaml
  label: officina.it Reports API
  slug: officina-it-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-reports-api-openapi.yml
- filename: officina-it-settings-api-openapi.yml
  format: yaml
  label: officina.it Settings API
  slug: officina-it-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-settings-api-openapi.yml
- filename: officina-it-suppliers-api-openapi.yml
  format: yaml
  label: officina.it Suppliers API
  slug: officina-it-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-suppliers-api-openapi.yml
- filename: officina-it-tyresets-api-openapi.yml
  format: yaml
  label: officina.it Tyre Sets API
  slug: officina-it-tyresets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-tyresets-api-openapi.yml
- filename: officina-it-vehicles-api-openapi.yml
  format: yaml
  label: officina.it Vehicles API
  slug: officina-it-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-vehicles-api-openapi.yml
- filename: officina-it-worksheets-api-openapi.yml
  format: yaml
  label: officina.it Worksheets API
  slug: officina-it-worksheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-worksheets-api-openapi.yml
- filename: officina-it-check-ins-api-openapi.yml
  format: yaml
  label: officina.it Check Ins API
  slug: officina-it-check-ins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-check-ins-api-openapi.yml
- filename: officina-it-time-tracking-api-openapi.yml
  format: yaml
  label: officina.it Time Tracking API
  slug: officina-it-time-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/officina-it/openapi/officina-it-time-tracking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: officina.it Authentication
name_suffix: Authentication
oauth_flows: []
overview: officina.it secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: officina.it
provider_slug: officina-it
scheme_count: 1
schemes:
- bearerFormat: APIKey
  description: 'Long-lived API key minted from Impostazioni → Accesso API.

    Format `ofk_live_<43 chars>` (`ofk_test_` outside production).

    Send it as `Authorization: Bearer ofk_live_…`.


    A key authorises a COMPANY and carries per-resource scopes;

    a call outside its scopes answers 403 `insufficient_scope`.

    Keys are shown once at creation and stored only as a digest.'
  name: PublicAPIKey
  scheme: bearer
  sources:
  - openapi/officina-it-openapi.json
  type: http
slug: officina-it-authentication
source_filename: officina-it-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/officina-it-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: PublicAPIKey\n  type: http\n  scheme: bearer\n  bearerFormat: APIKey\n  description: |-\n    Long-lived API key minted from Impostazioni → Accesso API.\n    Format `ofk_live_<43 chars>` (`ofk_test_` outside production).\n    Send it as `Authorization: Bearer ofk_live_…`.\n\n    A key authorises a COMPANY and carries per-resource scopes;\n    a call outside its scopes answers 403 `insufficient_scope`.\n    Keys are shown once at creation and stored only as a digest.\n  sources:\n  - openapi/officina-it-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/officina-it/authentication/officina-it-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Software-as-a-Service
- Management
- Italian
---
