---
api_key_in: []
api_specs:
- filename: fund-that-flip-activity-log-api-openapi.yml
  format: yaml
  label: Fund That Flip Activity Log API
  slug: fund-that-flip-activity-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-activity-log-api-openapi.yml
- filename: fund-that-flip-attachment-upload-api-openapi.yml
  format: yaml
  label: Fund That Flip Attachment Upload API
  slug: fund-that-flip-attachment-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-attachment-upload-api-openapi.yml
- filename: fund-that-flip-company-api-openapi.yml
  format: yaml
  label: Fund That Flip Company API
  slug: fund-that-flip-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-company-api-openapi.yml
- filename: fund-that-flip-company-categories-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Company: Categories API'
  slug: fund-that-flip-company-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-company-categories-api-openapi.yml
- filename: fund-that-flip-expense-accounts-api-openapi.yml
  format: yaml
  label: Fund That Flip Expense Accounts API
  slug: fund-that-flip-expense-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-expense-accounts-api-openapi.yml
- filename: fund-that-flip-project-api-openapi.yml
  format: yaml
  label: Fund That Flip Project API
  slug: fund-that-flip-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-api-openapi.yml
- filename: fund-that-flip-project-expenses-categories-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Project Expenses: Categories API'
  slug: fund-that-flip-project-expenses-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-expenses-categories-api-openapi.yml
- filename: fund-that-flip-project-expenses-line-items-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Project Expenses: Line Items API'
  slug: fund-that-flip-project-expenses-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-expenses-line-items-api-openapi.yml
- filename: fund-that-flip-project-expenses-transactions-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Project Expenses: Transactions API'
  slug: fund-that-flip-project-expenses-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-expenses-transactions-api-openapi.yml
- filename: fund-that-flip-project-income-api-openapi.yml
  format: yaml
  label: Fund That Flip Project Income API
  slug: fund-that-flip-project-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-income-api-openapi.yml
- filename: fund-that-flip-project-photo-log-photos-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Project Photo Log: Photos API'
  slug: fund-that-flip-project-photo-log-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-photo-log-photos-api-openapi.yml
- filename: fund-that-flip-project-receipts-api-openapi.yml
  format: yaml
  label: Fund That Flip Project Receipts API
  slug: fund-that-flip-project-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-receipts-api-openapi.yml
- filename: fund-that-flip-project-updates-api-openapi.yml
  format: yaml
  label: Fund That Flip Project Updates API
  slug: fund-that-flip-project-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-updates-api-openapi.yml
- filename: fund-that-flip-project-updates-photos-api-openapi.yml
  format: yaml
  label: 'Fund That Flip Project Updates: Photos API'
  slug: fund-that-flip-project-updates-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-project-updates-photos-api-openapi.yml
- filename: fund-that-flip-user-api-openapi.yml
  format: yaml
  label: Fund That Flip User API
  slug: fund-that-flip-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/openapi/fund-that-flip-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fund That Flip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fund That Flip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fund That Flip
provider_slug: fund-that-flip
scheme_count: 1
schemes:
- bearerFormat: FlipperForce Public API key
  description: 'Use the Public API key provided by FlipperForce as a Bearer token. Send the key exactly as provided in the Authorization header: `Authorization: Bearer <api-key>`.'
  name: PublicApiBearerAuth
  scheme: bearer
  sources:
  - openapi/fund-that-flip-flipperforce-public-api.yml
  type: http
slug: fund-that-flip-authentication
source_filename: fund-that-flip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: derived\nsource: openapi/fund-that-flip-flipperforce-public-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: PublicApiBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: FlipperForce Public API key\n  description: 'Use the Public API key provided by FlipperForce as a Bearer token. Send the\n    key exactly as provided in the Authorization header: `Authorization: Bearer <api-key>`.'\n  sources:\n  - openapi/fund-that-flip-flipperforce-public-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fund-that-flip/refs/heads/main/authentication/fund-that-flip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real-Estate
- Lending
- Construction
- Project Management
- Financial-Services
- Investing
- Fintech
- Property Technology
- Accounting
---
