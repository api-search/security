---
api_key_in: []
api_specs:
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Transactions API
  slug: navan-expense-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Fees and Adjustments API
  slug: navan-expense-fees-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Receipts API
  slug: navan-expense-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Custom Fields API
  slug: navan-expense-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Users API
  slug: navan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Bookings API
  slug: navan-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Webhooks API
  slug: navan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Navan Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Navan secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Navan
provider_slug: navan
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client-credentials flow. Generate a client_id / client_secret in the Navan app under Settings > Integrations (API), then POST grant_type=client_credentials to the token URL to obtain a Bearer access token. US token URL: https://app.navan.com/ta-auth/oauth/token ; EU token URL: https://app-fra.navan.com/ta-auth/oauth/token . (Some integrations reference an https://api.navan.com/ta-auth/oa'
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://app.navan.com/ta-auth/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/navan-openapi.yml
  type: oauth2
slug: navan-authentication
source_filename: navan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/navan-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.navan.com/ta-auth/oauth/token\n    scopes: 6\n  description: 'OAuth 2.0 client-credentials flow. Generate a client_id / client_secret in the\n    Navan app under Settings > Integrations (API), then POST grant_type=client_credentials to\n    the token URL to obtain a Bearer access token. US token URL: https://app.navan.com/ta-auth/oauth/token\n    ; EU token URL: https://app-fra.navan.com/ta-auth/oauth/token . (Some integrations reference\n    an https://api.navan.com/ta-auth/oa'\n  sources:\n  - openapi/navan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/authentication/navan-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Corporate Travel
- Expense Management
- Corporate Cards
- Spend Management
- T&E
- Fintech
- Business Travel
---
