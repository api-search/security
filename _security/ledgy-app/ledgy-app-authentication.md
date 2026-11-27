---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ledgy-app-accounts-api-openapi.yml
  format: yaml
  label: Ledgy Accounts API
  slug: ledgy-app-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-accounts-api-openapi.yml
- filename: ledgy-app-budgets-api-openapi.yml
  format: yaml
  label: Ledgy Budgets API
  slug: ledgy-app-budgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-budgets-api-openapi.yml
- filename: ledgy-app-categories-api-openapi.yml
  format: yaml
  label: Ledgy Categories API
  slug: ledgy-app-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-categories-api-openapi.yml
- filename: ledgy-app-groupmembers-api-openapi.yml
  format: yaml
  label: Ledgy Group Members API
  slug: ledgy-app-groupmembers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-groupmembers-api-openapi.yml
- filename: ledgy-app-groups-api-openapi.yml
  format: yaml
  label: Ledgy Groups API
  slug: ledgy-app-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-groups-api-openapi.yml
- filename: ledgy-app-icons-api-openapi.yml
  format: yaml
  label: Ledgy Icons API
  slug: ledgy-app-icons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-icons-api-openapi.yml
- filename: ledgy-app-recurringtransactions-api-openapi.yml
  format: yaml
  label: Ledgy Recurring Transactions API
  slug: ledgy-app-recurringtransactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-recurringtransactions-api-openapi.yml
- filename: ledgy-app-reports-api-openapi.yml
  format: yaml
  label: Ledgy Reports API
  slug: ledgy-app-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-reports-api-openapi.yml
- filename: ledgy-app-settlements-api-openapi.yml
  format: yaml
  label: Ledgy Settlements API
  slug: ledgy-app-settlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-settlements-api-openapi.yml
- filename: ledgy-app-transactions-api-openapi.yml
  format: yaml
  label: Ledgy Transactions API
  slug: ledgy-app-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-transactions-api-openapi.yml
- filename: ledgy-app-user-settings-api-openapi.yml
  format: yaml
  label: Ledgy User Settings API
  slug: ledgy-app-user-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgy-app/openapi/ledgy-app-user-settings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ledgy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledgy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ledgy
provider_slug: ledgy-app
scheme_count: 1
schemes:
- description: 'JWT or Personal Access Token. For JWT: "Bearer {jwt_token}". For PAT: "Bearer lgpat_{token}"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/swagger.json
  type: apiKey
slug: ledgy-app-authentication
source_filename: ledgy-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/swagger.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT or Personal Access Token. For JWT: \"Bearer {jwt_token}\". For PAT: \"Bearer\n    lgpat_{token}\"'\n  sources:\n  - openapi/swagger.json\n"
source_yaml_url: https://artifacts.apis.io/ledgy-app/authentication/ledgy-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Expense Tracking
- iOS
- Artificial Intelligence
- Multi-Currency
---
