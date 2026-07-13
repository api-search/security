---
api_key_in:
- header
api_specs:
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Companies API
  slug: puzzle-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Transactions API
  slug: puzzle-io-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Ledger Accounts API
  slug: puzzle-io-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Journal Entries API
  slug: puzzle-io-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Financial Reports API
  slug: puzzle-io-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Metrics API
  slug: puzzle-io-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Categories API
  slug: puzzle-io-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Integrations API
  slug: puzzle-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Puzzle Io Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Puzzle secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Puzzle
provider_slug: puzzle-io
scheme_count: 2
schemes:
- description: OAuth 2.0 with scoped access (for example read:company, read:transactions, read:report). Partner credentials are issued after the Puzzle partner technical review.
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://puzzle-api.readme.io/reference
  name: oauth2
  sources:
  - openapi/puzzle-io-openapi.yml
  type: oauth2
- description: API key authentication via the Authorization header, as described in the Puzzle developer docs.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/puzzle-io-openapi.yml
  type: apiKey
slug: puzzle-io-authentication
source_filename: puzzle-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/puzzle-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://puzzle-api.readme.io/reference\n    scopes: 4\n  description: OAuth 2.0 with scoped access (for example read:company, read:transactions, read:report).\n    Partner credentials are issued after the Puzzle partner technical review.\n  sources:\n  - openapi/puzzle-io-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication via the Authorization header, as described in the Puzzle\n    developer docs.\n  sources:\n  - openapi/puzzle-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/authentication/puzzle-io-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Accounting
- Fintech
- General Ledger
- Financial Reporting
- Bookkeeping
- Startups
- Embedded Accounting
- Metrics
---
