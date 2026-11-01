---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: end-close-bank-account-balances-api-openapi.yml
  format: yaml
  label: End Close Bank Account Balances API
  slug: end-close-bank-account-balances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-bank-account-balances-api-openapi.yml
- filename: end-close-bank-accounts-api-openapi.yml
  format: yaml
  label: End Close Bank Accounts API
  slug: end-close-bank-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-bank-accounts-api-openapi.yml
- filename: end-close-bulk-requests-api-openapi.yml
  format: yaml
  label: End Close Bulk Requests API
  slug: end-close-bulk-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-bulk-requests-api-openapi.yml
- filename: end-close-data-stream-property-definitions-api-openapi.yml
  format: yaml
  label: End Close Data Stream Property Definitions API
  slug: end-close-data-stream-property-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-data-stream-property-definitions-api-openapi.yml
- filename: end-close-data-streams-api-openapi.yml
  format: yaml
  label: End Close Data Streams API
  slug: end-close-data-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-data-streams-api-openapi.yml
- filename: end-close-reconciliation-exceptions-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Exceptions API
  slug: end-close-reconciliation-exceptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-reconciliation-exceptions-api-openapi.yml
- filename: end-close-reconciliation-matches-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Matches API
  slug: end-close-reconciliation-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-reconciliation-matches-api-openapi.yml
- filename: end-close-reconciliation-rules-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Rules API
  slug: end-close-reconciliation-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-reconciliation-rules-api-openapi.yml
- filename: end-close-reconciliation-stories-api-openapi.yml
  format: yaml
  label: End Close Reconciliation Stories API
  slug: end-close-reconciliation-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-reconciliation-stories-api-openapi.yml
- filename: end-close-reconciliations-api-openapi.yml
  format: yaml
  label: End Close Reconciliations API
  slug: end-close-reconciliations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-reconciliations-api-openapi.yml
- filename: end-close-records-api-openapi.yml
  format: yaml
  label: End Close Records API
  slug: end-close-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-records-api-openapi.yml
- filename: end-close-end-close-api-api-openapi.yml
  format: yaml
  label: End Close End Close API
  slug: end-close-end-close-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-end-close-api-api-openapi.yml
- filename: end-close-agents-api-openapi.yml
  format: yaml
  label: End Close Agents API
  slug: end-close-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-agents-api-openapi.yml
- filename: end-close-file-imports-api-openapi.yml
  format: yaml
  label: End Close File Imports API
  slug: end-close-file-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-file-imports-api-openapi.yml
- filename: end-close-relays-api-openapi.yml
  format: yaml
  label: End Close Relays API
  slug: end-close-relays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/end-close/openapi/end-close-relays-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: End Close Authentication
name_suffix: Authentication
oauth_flows: []
overview: End Close secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: End Close
provider_slug: end-close
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/end-close-openapi-original.json
  type: apiKey
slug: end-close-authentication
source_filename: end-close-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/end-close-openapi-original.json\ndocs: https://endclose.com/docs/authentication.md\nnotes: >-\n  End Close authenticates every request with an API key sent in the X-API-KEY header.\n  Keys are viewed/managed in the Settings section of the End Close dashboard\n  (https://app.endclose.com). Keys are environment-scoped (test vs live).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/end-close-openapi-original.json\n"
source_yaml_url: https://artifacts.apis.io/end-close/authentication/end-close-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Reconciliation
- Payments
- Financial Operations
- Accounting
- Banking
- Data Integration
- Webhook
- Fintech
---
