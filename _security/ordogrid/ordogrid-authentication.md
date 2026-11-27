---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ordogrid-clients-api-openapi.yml
  format: yaml
  label: OrdoGrid Clients API
  slug: ordogrid-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-clients-api-openapi.yml
- filename: ordogrid-credit-notes-api-openapi.yml
  format: yaml
  label: OrdoGrid Credit Notes API
  slug: ordogrid-credit-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-credit-notes-api-openapi.yml
- filename: ordogrid-fidelity-api-openapi.yml
  format: yaml
  label: OrdoGrid Fidelity API
  slug: ordogrid-fidelity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-fidelity-api-openapi.yml
- filename: ordogrid-invoices-api-openapi.yml
  format: yaml
  label: OrdoGrid Invoices API
  slug: ordogrid-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-invoices-api-openapi.yml
- filename: ordogrid-meta-api-openapi.yml
  format: yaml
  label: OrdoGrid Meta API
  slug: ordogrid-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-meta-api-openapi.yml
- filename: ordogrid-payments-api-openapi.yml
  format: yaml
  label: OrdoGrid Payments API
  slug: ordogrid-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-payments-api-openapi.yml
- filename: ordogrid-peppol-api-openapi.yml
  format: yaml
  label: OrdoGrid Peppol API
  slug: ordogrid-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-peppol-api-openapi.yml
- filename: ordogrid-quotes-api-openapi.yml
  format: yaml
  label: OrdoGrid Quotes API
  slug: ordogrid-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-quotes-api-openapi.yml
- filename: ordogrid-receipts-api-openapi.yml
  format: yaml
  label: OrdoGrid Receipts API
  slug: ordogrid-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-receipts-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OrdoGrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: OrdoGrid secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OrdoGrid
provider_slug: ordogrid
scheme_count: 2
schemes:
- bearerFormat: API key
  description: Company-scoped key prefixed ik_live_. Create it in Company → API keys. X-Api-Key is also accepted.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/ordogrid-openapi.json
  type: http
- description: 'Alternative to Authorization: Bearer.'
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ordogrid-openapi.json
  type: apiKey
slug: ordogrid-authentication
source_filename: ordogrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/ordogrid-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: Company-scoped key prefixed ik_live_. Create it in Company → API keys. X-Api-Key\n    is also accepted.\n  sources:\n  - openapi/ordogrid-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Alternative to Authorization: Bearer.'\n  sources:\n  - openapi/ordogrid-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ordogrid/authentication/ordogrid-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Invoicing
- Peppol
- Belgium
- Software-as-a-Service
- business-documents
---
