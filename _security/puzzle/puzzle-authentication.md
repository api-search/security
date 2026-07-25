---
api_key_in: []
api_specs:
- filename: puzzle-accounts-api-openapi.yml
  format: yaml
  label: Puzzle Accounts API
  slug: puzzle-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-accounts-api-openapi.yml
- filename: puzzle-attachments-api-openapi.yml
  format: yaml
  label: Puzzle Attachments API
  slug: puzzle-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-attachments-api-openapi.yml
- filename: puzzle-bills-api-openapi.yml
  format: yaml
  label: Puzzle Bills API
  slug: puzzle-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-bills-api-openapi.yml
- filename: puzzle-company-api-openapi.yml
  format: yaml
  label: Puzzle Company API
  slug: puzzle-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-company-api-openapi.yml
- filename: puzzle-customers-api-openapi.yml
  format: yaml
  label: Puzzle Customers API
  slug: puzzle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-customers-api-openapi.yml
- filename: puzzle-departments-api-openapi.yml
  format: yaml
  label: Puzzle Departments API
  slug: puzzle-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-departments-api-openapi.yml
- filename: puzzle-documents-api-openapi.yml
  format: yaml
  label: Puzzle Documents API
  slug: puzzle-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-documents-api-openapi.yml
- filename: puzzle-invoices-api-openapi.yml
  format: yaml
  label: Puzzle Invoices API
  slug: puzzle-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-invoices-api-openapi.yml
- filename: puzzle-journalentries-api-openapi.yml
  format: yaml
  label: Puzzle JournalEntries API
  slug: puzzle-journalentries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-journalentries-api-openapi.yml
- filename: puzzle-journalentry-api-openapi.yml
  format: yaml
  label: Puzzle JournalEntry API
  slug: puzzle-journalentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-journalentry-api-openapi.yml
- filename: puzzle-locations-api-openapi.yml
  format: yaml
  label: Puzzle Locations API
  slug: puzzle-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-locations-api-openapi.yml
- filename: puzzle-metrics-api-openapi.yml
  format: yaml
  label: Puzzle Metrics API
  slug: puzzle-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-metrics-api-openapi.yml
- filename: puzzle-oauth-api-openapi.yml
  format: yaml
  label: Puzzle OAuth API
  slug: puzzle-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-oauth-api-openapi.yml
- filename: puzzle-onboarding-api-openapi.yml
  format: yaml
  label: Puzzle Onboarding API
  slug: puzzle-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-onboarding-api-openapi.yml
- filename: puzzle-payroll-api-openapi.yml
  format: yaml
  label: Puzzle Payroll API
  slug: puzzle-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-payroll-api-openapi.yml
- filename: puzzle-products-api-openapi.yml
  format: yaml
  label: Puzzle Products API
  slug: puzzle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-products-api-openapi.yml
- filename: puzzle-reports-api-openapi.yml
  format: yaml
  label: Puzzle Reports API
  slug: puzzle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-reports-api-openapi.yml
- filename: puzzle-requests-api-openapi.yml
  format: yaml
  label: Puzzle Requests API
  slug: puzzle-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-requests-api-openapi.yml
- filename: puzzle-tasks-api-openapi.yml
  format: yaml
  label: Puzzle Tasks API
  slug: puzzle-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-tasks-api-openapi.yml
- filename: puzzle-transactions-api-openapi.yml
  format: yaml
  label: Puzzle Transactions API
  slug: puzzle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-transactions-api-openapi.yml
- filename: puzzle-user-api-openapi.yml
  format: yaml
  label: Puzzle User API
  slug: puzzle-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-user-api-openapi.yml
- filename: puzzle-vendors-api-openapi.yml
  format: yaml
  label: Puzzle Vendors API
  slug: puzzle-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-vendors-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Puzzle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Puzzle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Puzzle
provider_slug: puzzle
scheme_count: 1
schemes:
- authorizationUrl: https://api.puzzle.io/oauth/authorize
  credentials:
  - client_id
  - client_secret
  - connection_key
  flow: authorizationCode
  name: OAuth2
  pkce: true
  refresh: refresh_token grant supported; offline_access scope for long-lived access
  sandbox_authorizationUrl: https://staging.southparkdata.com/oauth/authorize
  sandbox_tokenUrl: https://staging.southparkdata.com/oauth/token
  scheme: oauth2
  tokenUrl: https://api.puzzle.io/oauth/token
  token_endpoint_auth: Clients may authenticate at the token endpoint via HTTP Basic (recommended for confidential clients) or by including client_id / client_secret in the x-www-form-urlencoded body.
  type: oauth2
slug: puzzle-authentication
source_filename: puzzle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://puzzle-api.readme.io/docs/getting-started\ndocs: https://puzzle-api.readme.io/docs/getting-started\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  legacy: link-token (deprecated)\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: oauth2\n  flow: authorizationCode\n  pkce: true\n  authorizationUrl: https://api.puzzle.io/oauth/authorize\n  tokenUrl: https://api.puzzle.io/oauth/token\n  sandbox_authorizationUrl: https://staging.southparkdata.com/oauth/authorize\n  sandbox_tokenUrl: https://staging.southparkdata.com/oauth/token\n  token_endpoint_auth: >-\n    Clients may authenticate at the token endpoint via HTTP Basic (recommended for\n    confidential clients) or by including client_id / client_secret in the\n    x-www-form-urlencoded body.\n  credentials:\n  - client_id\n  - client_secret\n  - connection_key\n  refresh: refresh_token grant supported; offline_access scope for long-lived\
  \ access\nnotes: >-\n  Authentication is OAuth 2.0 Authorization Code flow with PKCE. Partners request a\n  client ID, client secret, and connection key from Puzzle (api@puzzle.io) and register\n  valid redirect URIs. A legacy link-token flow exists for existing partners but is\n  deprecated in favor of OAuth. The current user can be identified via the /me endpoint,\n  valid only for OAuth connections. The OpenAPI document does not declare securitySchemes;\n  this profile is captured from the developer documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/authentication/puzzle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Accounting
- Financial
- Bookkeeping
- Fintech
- General Ledger
- Payroll
- Agent-Native
- MCP
---
