---
api_key_in:
- header
api_specs:
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Owners API
  slug: gingr-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Pets API
  slug: gingr-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Reservations API
  slug: gingr-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Services API
  slug: gingr-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Invoices & Payments API
  slug: gingr-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Vaccinations API
  slug: gingr-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Report Cards API
  slug: gingr-report-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Waitlist API
  slug: gingr-waitlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/authentication/gingr-authentication.yml
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
