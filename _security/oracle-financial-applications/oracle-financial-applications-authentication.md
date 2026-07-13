---
api_key_in: []
api_specs:
- filename: op-version-latest-get.html
  format: yaml
  label: Oracle ERP Cloud REST API
  slug: oracle-erp-cloud-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/24d/farfa/op-version-latest-get.html
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
