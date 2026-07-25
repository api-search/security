---
api_key_in: []
api_specs:
- filename: oracle-general-ledger-accounting-periods-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Accounting Periods API
  slug: oracle-general-ledger-accounting-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-accounting-periods-api-openapi.yml
- filename: oracle-general-ledger-budgetary-control-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Budgetary Control API
  slug: oracle-general-ledger-budgetary-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-budgetary-control-api-openapi.yml
- filename: oracle-general-ledger-currency-rates-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Currency Rates API
  slug: oracle-general-ledger-currency-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-currency-rates-api-openapi.yml
- filename: oracle-general-ledger-erp-integrations-api-openapi.yml
  format: yaml
  label: Oracle General Ledger ERP Integrations API
  slug: oracle-general-ledger-erp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-erp-integrations-api-openapi.yml
- filename: oracle-general-ledger-intercompany-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Intercompany API
  slug: oracle-general-ledger-intercompany-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-intercompany-api-openapi.yml
- filename: oracle-general-ledger-journal-batches-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Journal Batches API
  slug: oracle-general-ledger-journal-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-journal-batches-api-openapi.yml
- filename: oracle-general-ledger-ledger-balances-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Ledger Balances API
  slug: oracle-general-ledger-ledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-ledger-balances-api-openapi.yml
- filename: oracle-general-ledger-ledger-options-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Ledger Options API
  slug: oracle-general-ledger-ledger-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-ledger-options-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle General Ledger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle General Ledger secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle General Ledger
provider_slug: oracle-general-ledger
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with Oracle Cloud user credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-general-ledger-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token from Oracle IDCS / IAM.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-general-ledger-openapi.yml
  type: http
slug: oracle-general-ledger-authentication
source_filename: oracle-general-ledger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-general-ledger-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with Oracle Cloud user credentials.\n  sources:\n  - openapi/oracle-general-ledger-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token from Oracle IDCS / IAM.\n  sources:\n  - openapi/oracle-general-ledger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/authentication/oracle-general-ledger-authentication.yml
summary_line: http · 2 schemes
tags:
- Accounting
- Balances
- Cloud
- ERP
- Finance
- General Ledger
- Journals
---
