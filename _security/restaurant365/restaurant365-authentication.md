---
api_key_in: []
api_specs:
- filename: restaurant365-ap-invoices-api-openapi.yml
  format: yaml
  label: Restaurant365 AP Invoices API
  slug: restaurant365-ap-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-ap-invoices-api-openapi.yml
- filename: restaurant365-audit-api-openapi.yml
  format: yaml
  label: Restaurant365 Audit API
  slug: restaurant365-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-audit-api-openapi.yml
- filename: restaurant365-authentication-api-openapi.yml
  format: yaml
  label: Restaurant365 Authentication API
  slug: restaurant365-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-authentication-api-openapi.yml
- filename: restaurant365-general-ledger-api-openapi.yml
  format: yaml
  label: Restaurant365 General Ledger API
  slug: restaurant365-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-general-ledger-api-openapi.yml
- filename: restaurant365-labor-api-openapi.yml
  format: yaml
  label: Restaurant365 Labor API
  slug: restaurant365-labor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-labor-api-openapi.yml
- filename: restaurant365-metadata-api-openapi.yml
  format: yaml
  label: Restaurant365 Metadata API
  slug: restaurant365-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-metadata-api-openapi.yml
- filename: restaurant365-reference-data-api-openapi.yml
  format: yaml
  label: Restaurant365 Reference Data API
  slug: restaurant365-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-reference-data-api-openapi.yml
- filename: restaurant365-sales-api-openapi.yml
  format: yaml
  label: Restaurant365 Sales API
  slug: restaurant365-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-sales-api-openapi.yml
- filename: restaurant365-transactions-api-openapi.yml
  format: yaml
  label: Restaurant365 Transactions API
  slug: restaurant365-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Restaurant365 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Restaurant365 secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Restaurant365
provider_slug: restaurant365
scheme_count: 2
schemes:
- description: Domain\Username with R365 password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/restaurant365-odata-connector-openapi.yml
  type: http
- description: Bearer token returned by the Authenticate operation
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/restaurant365-r365-api-openapi.yml
  type: http
slug: restaurant365-authentication
source_filename: restaurant365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restaurant365-odata-connector-openapi.yml, openapi/restaurant365-r365-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Domain\\Username with R365 password\n  sources:\n  - openapi/restaurant365-odata-connector-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token returned by the Authenticate operation\n  sources:\n  - openapi/restaurant365-r365-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/authentication/restaurant365-authentication.yml
summary_line: http · 2 schemes
tags:
- Restaurant
- Accounting
- Inventory
- Operations
- Invoices
- Reporting
- OData
---
