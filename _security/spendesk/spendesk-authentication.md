---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spendesk-accounting-exports-api-openapi.yml
  format: yaml
  label: Spendesk Accounting exports API
  slug: spendesk-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-accounting-exports-api-openapi.yml
- filename: spendesk-analytical-fields-and-cost-centers-api-openapi.yml
  format: yaml
  label: Spendesk Analytical fields and cost centers API
  slug: spendesk-analytical-fields-and-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-analytical-fields-and-cost-centers-api-openapi.yml
- filename: spendesk-authentication-api-openapi.yml
  format: yaml
  label: Spendesk Authentication API
  slug: spendesk-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-authentication-api-openapi.yml
- filename: spendesk-cards-api-openapi.yml
  format: yaml
  label: Spendesk Cards API
  slug: spendesk-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-cards-api-openapi.yml
- filename: spendesk-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Spendesk Chart of accounts API
  slug: spendesk-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-chart-of-accounts-api-openapi.yml
- filename: spendesk-companies-api-openapi.yml
  format: yaml
  label: Spendesk Companies API
  slug: spendesk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-companies-api-openapi.yml
- filename: spendesk-expense-categories-api-openapi.yml
  format: yaml
  label: Spendesk Expense categories API
  slug: spendesk-expense-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-expense-categories-api-openapi.yml
- filename: spendesk-external-references-api-openapi.yml
  format: yaml
  label: Spendesk External references API
  slug: spendesk-external-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-external-references-api-openapi.yml
- filename: spendesk-invoices-and-intakes-api-openapi.yml
  format: yaml
  label: Spendesk Invoices and intakes API
  slug: spendesk-invoices-and-intakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-invoices-and-intakes-api-openapi.yml
- filename: spendesk-mcp-api-openapi.yml
  format: yaml
  label: Spendesk MCP API
  slug: spendesk-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-mcp-api-openapi.yml
- filename: spendesk-payables-api-openapi.yml
  format: yaml
  label: Spendesk Payables API
  slug: spendesk-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-payables-api-openapi.yml
- filename: spendesk-purchase-orders-api-openapi.yml
  format: yaml
  label: Spendesk Purchase orders API
  slug: spendesk-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-purchase-orders-api-openapi.yml
- filename: spendesk-requests-and-transactions-api-openapi.yml
  format: yaml
  label: Spendesk Requests and transactions API
  slug: spendesk-requests-and-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-requests-and-transactions-api-openapi.yml
- filename: spendesk-settlements-and-wallet-api-openapi.yml
  format: yaml
  label: Spendesk Settlements and wallet API
  slug: spendesk-settlements-and-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-settlements-and-wallet-api-openapi.yml
- filename: spendesk-spendesk-public-api-api-openapi.yml
  format: yaml
  label: Spendesk Spendesk Public API
  slug: spendesk-spendesk-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-spendesk-public-api-api-openapi.yml
- filename: spendesk-suppliers-api-openapi.yml
  format: yaml
  label: Spendesk Suppliers API
  slug: spendesk-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-suppliers-api-openapi.yml
- filename: spendesk-users-api-openapi.yml
  format: yaml
  label: Spendesk Users API
  slug: spendesk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-users-api-openapi.yml
- filename: spendesk-webhooks-api-openapi.yml
  format: yaml
  label: Spendesk Webhooks API
  slug: spendesk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/openapi/spendesk-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Spendesk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Spendesk secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Spendesk
provider_slug: spendesk
scheme_count: 1
schemes:
- description: 'A company-level token acts on the company it was issued for. An organisation-level token (experimental) acts on the companies of an organisation: send the target company in the `X-Company-Id` header on every call, except on `GET /v2/companies` and on `/v2/companies/{companyId}/…` routes, which carry the company in the path. See [Organisation-level access](/reference/organisation-level-access).'
  flows:
  - flow: clientCredentials
    scopes: 39
    tokenUrl: /v1/auth/token
  - authorizationUrl: /v1/oauth2/authorize
    flow: authorizationCode
    scopes: 39
    tokenUrl: /v1/oauth2/token/create
  name: Authentication
  sources:
  - openapi/spendesk-public-api-openapi.yml
  type: oauth2
slug: spendesk-authentication
source_filename: spendesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/spendesk-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: Authentication\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n    scopes: 39\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth2/authorize\n    tokenUrl: /v1/oauth2/token/create\n    scopes: 39\n  description: 'A company-level token acts on the company it was issued for. An organisation-level\n    token (experimental) acts on the companies of an organisation: send the target company in\n    the `X-Company-Id` header on every call, except on `GET /v2/companies` and on `/v2/companies/{companyId}/…`\n    routes, which carry the company in the path. See [Organisation-level access](/reference/organisation-level-access).'\n  sources:\n  - openapi/spendesk-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/authentication/spendesk-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Spend Management
- Corporate Cards
- Expense Management
- Invoices
- Procurement
- Fintech
- Accounting
- Payments
---
