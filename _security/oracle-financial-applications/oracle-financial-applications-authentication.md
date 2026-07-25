---
api_key_in: []
api_specs:
- filename: oracle-financial-applications-cash-management-api-openapi.yml
  format: yaml
  label: Oracle Financial Applications Cash Management API
  slug: oracle-financial-applications-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/openapi/oracle-financial-applications-cash-management-api-openapi.yml
- filename: oracle-financial-applications-fixed-assets-api-openapi.yml
  format: yaml
  label: Oracle Financial Applications Fixed Assets API
  slug: oracle-financial-applications-fixed-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/openapi/oracle-financial-applications-fixed-assets-api-openapi.yml
- filename: oracle-financial-applications-general-ledger-api-openapi.yml
  format: yaml
  label: Oracle Financial Applications General Ledger API
  slug: oracle-financial-applications-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/openapi/oracle-financial-applications-general-ledger-api-openapi.yml
- filename: oracle-financial-applications-payables-api-openapi.yml
  format: yaml
  label: Oracle Financial Applications Payables API
  slug: oracle-financial-applications-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/openapi/oracle-financial-applications-payables-api-openapi.yml
- filename: oracle-financial-applications-receivables-api-openapi.yml
  format: yaml
  label: Oracle Financial Applications Receivables API
  slug: oracle-financial-applications-receivables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/openapi/oracle-financial-applications-receivables-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Financial Applications Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Financial Applications secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Financial Applications
provider_slug: oracle-financial-applications
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with Oracle Cloud user credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-financial-applications-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token from Oracle IDCS / IAM.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-financial-applications-openapi.yml
  type: http
slug: oracle-financial-applications-authentication
source_filename: oracle-financial-applications-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-financial-applications-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with Oracle Cloud user credentials.\n  sources:\n  - openapi/oracle-financial-applications-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token from Oracle IDCS / IAM.\n  sources:\n  - openapi/oracle-financial-applications-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/authentication/oracle-financial-applications-authentication.yml
summary_line: http · 2 schemes
tags:
- Accounting
- Cloud Applications
- Enterprise Performance Management
- Enterprise Resource Planning
- EPM
- ERP
- Financial Management
- Financial Reporting
---
