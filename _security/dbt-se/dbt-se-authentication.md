---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dbt-se-agents-api-openapi.yml
  format: yaml
  label: DBT Capital Agents API
  slug: dbt-se-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-agents-api-openapi.yml
- filename: dbt-se-banking-api-openapi.yml
  format: yaml
  label: DBT Capital Banking API
  slug: dbt-se-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-banking-api-openapi.yml
- filename: dbt-se-bookkeeping-api-openapi.yml
  format: yaml
  label: DBT Capital Bookkeeping API
  slug: dbt-se-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-bookkeeping-api-openapi.yml
- filename: dbt-se-documents-api-openapi.yml
  format: yaml
  label: DBT Capital Documents API
  slug: dbt-se-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-documents-api-openapi.yml
- filename: dbt-se-files-api-openapi.yml
  format: yaml
  label: DBT Capital Files API
  slug: dbt-se-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-files-api-openapi.yml
- filename: dbt-se-identity-api-openapi.yml
  format: yaml
  label: DBT Capital Identity API
  slug: dbt-se-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-identity-api-openapi.yml
- filename: dbt-se-llm-api-openapi.yml
  format: yaml
  label: DBT Capital LLM API
  slug: dbt-se-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-llm-api-openapi.yml
- filename: dbt-se-notification-api-openapi.yml
  format: yaml
  label: DBT Capital Notification API
  slug: dbt-se-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-notification-api-openapi.yml
- filename: dbt-se-portfolio-api-openapi.yml
  format: yaml
  label: DBT Capital Portfolio API
  slug: dbt-se-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-portfolio-api-openapi.yml
- filename: dbt-se-prospect-api-openapi.yml
  format: yaml
  label: DBT Capital Prospect API
  slug: dbt-se-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-prospect-api-openapi.yml
- filename: dbt-se-regulatory-records-api-openapi.yml
  format: yaml
  label: DBT Capital Regulatory Records API
  slug: dbt-se-regulatory-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-regulatory-records-api-openapi.yml
- filename: dbt-se-uc-api-openapi.yml
  format: yaml
  label: DBT Capital UC API
  slug: dbt-se-uc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-uc-api-openapi.yml
- filename: dbt-se-upload-api-openapi.yml
  format: yaml
  label: DBT Capital Upload API
  slug: dbt-se-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-upload-api-openapi.yml
- filename: dbt-se-workbooks-api-openapi.yml
  format: yaml
  label: DBT Capital Workbooks API
  slug: dbt-se-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/openapi/dbt-se-workbooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dbt Se Authentication
name_suffix: Authentication
oauth_flows: []
overview: DBT Capital secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DBT Capital
provider_slug: dbt-se
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: JWT Bearer
  scheme: bearer
  sources:
  - openapi/dbt-se-openapi.json
  type: http
- name: Cookie
  scheme: cookie
  sources:
  - openapi/dbt-se-openapi.json
  type: http
slug: dbt-se-authentication
source_filename: dbt-se-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/dbt-se-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dbt-se-openapi.json\n- name: Cookie\n  type: http\n  scheme: cookie\n  sources:\n  - openapi/dbt-se-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbt-se/refs/heads/main/authentication/dbt-se-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Finance
- Loans
- Sweden
- Business
---
