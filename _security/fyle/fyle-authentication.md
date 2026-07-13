---
api_key_in: []
api_specs:
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Expenses API
  slug: fyle-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Reports API
  slug: fyle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Advances API
  slug: fyle-advances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Categories API
  slug: fyle-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Projects API
  slug: fyle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Cost Centers API
  slug: fyle-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Employees API
  slug: fyle-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Merchants API
  slug: fyle-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Corporate Cards & Transactions API
  slug: fyle-corporate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Webhooks API
  slug: fyle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Files & Receipts API
  slug: fyle-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fyle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fyle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fyle
provider_slug: fyle
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 Bearer access token. Obtain it via the refresh-token grant at the Fyle OAuth token endpoint (accounts host) using your client_id, client_secret, and refresh_token, then send it as `Authorization: Bearer <access_token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fyle-openapi.yml
  type: http
slug: fyle-authentication
source_filename: fyle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fyle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth 2.0 Bearer access token. Obtain it via the refresh-token grant at the\n    Fyle OAuth token endpoint (accounts host) using your client_id, client_secret, and refresh_token,\n    then send it as `Authorization: Bearer <access_token>`.'\n  sources:\n  - openapi/fyle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/authentication/fyle-authentication.yml
summary_line: http · 1 scheme
tags:
- Expense Management
- Spend Management
- Corporate Cards
- Fintech
- Accounting
- Receipts
---
