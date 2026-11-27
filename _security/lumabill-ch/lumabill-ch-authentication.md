---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumabill-ch-account-api-openapi.yml
  format: yaml
  label: LumaBill Account API
  slug: lumabill-ch-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-account-api-openapi.yml
- filename: lumabill-ch-bank-accounts-api-openapi.yml
  format: yaml
  label: LumaBill Bank Accounts API
  slug: lumabill-ch-bank-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-bank-accounts-api-openapi.yml
- filename: lumabill-ch-bank-imports-api-openapi.yml
  format: yaml
  label: LumaBill Bank Imports API
  slug: lumabill-ch-bank-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-bank-imports-api-openapi.yml
- filename: lumabill-ch-catalog-api-openapi.yml
  format: yaml
  label: LumaBill Catalog API
  slug: lumabill-ch-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-catalog-api-openapi.yml
- filename: lumabill-ch-chart-of-accounts-api-openapi.yml
  format: yaml
  label: LumaBill Chart of Accounts API
  slug: lumabill-ch-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-chart-of-accounts-api-openapi.yml
- filename: lumabill-ch-clients-api-openapi.yml
  format: yaml
  label: LumaBill Clients API
  slug: lumabill-ch-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-clients-api-openapi.yml
- filename: lumabill-ch-expenses-api-openapi.yml
  format: yaml
  label: LumaBill Expenses API
  slug: lumabill-ch-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-expenses-api-openapi.yml
- filename: lumabill-ch-fiscal-years-api-openapi.yml
  format: yaml
  label: LumaBill Fiscal Years API
  slug: lumabill-ch-fiscal-years-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-fiscal-years-api-openapi.yml
- filename: lumabill-ch-invoices-api-openapi.yml
  format: yaml
  label: LumaBill Invoices API
  slug: lumabill-ch-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-invoices-api-openapi.yml
- filename: lumabill-ch-journal-entries-api-openapi.yml
  format: yaml
  label: LumaBill Journal Entries API
  slug: lumabill-ch-journal-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-journal-entries-api-openapi.yml
- filename: lumabill-ch-offers-api-openapi.yml
  format: yaml
  label: LumaBill Offers API
  slug: lumabill-ch-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-offers-api-openapi.yml
- filename: lumabill-ch-payments-api-openapi.yml
  format: yaml
  label: LumaBill Payments API
  slug: lumabill-ch-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-payments-api-openapi.yml
- filename: lumabill-ch-profiles-api-openapi.yml
  format: yaml
  label: LumaBill Profiles API
  slug: lumabill-ch-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-profiles-api-openapi.yml
- filename: lumabill-ch-recurring-invoices-api-openapi.yml
  format: yaml
  label: LumaBill Recurring Invoices API
  slug: lumabill-ch-recurring-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-recurring-invoices-api-openapi.yml
- filename: lumabill-ch-reports-api-openapi.yml
  format: yaml
  label: LumaBill Reports API
  slug: lumabill-ch-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-reports-api-openapi.yml
- filename: lumabill-ch-revenue-api-openapi.yml
  format: yaml
  label: LumaBill Revenue API
  slug: lumabill-ch-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-revenue-api-openapi.yml
- filename: lumabill-ch-vendors-api-openapi.yml
  format: yaml
  label: LumaBill Vendors API
  slug: lumabill-ch-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LumaBill Authentication
name_suffix: Authentication
oauth_flows: []
overview: LumaBill secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LumaBill
provider_slug: lumabill-ch
scheme_count: 1
schemes:
- bearerFormat: lmb_...
  description: API key obtained from Lumabill dashboard → Settings → API Keys
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lumabill-ch-openapi.yaml
  type: http
slug: lumabill-ch-authentication
source_filename: lumabill-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lumabill-ch-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: lmb_...\n  description: API key obtained from Lumabill dashboard → Settings → API Keys\n  sources:\n  - openapi/lumabill-ch-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/lumabill-ch/authentication/lumabill-ch-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Invoicing
- Software-as-a-Service
- Switzerland
- Small Business
---
