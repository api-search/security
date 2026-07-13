---
api_key_in: []
api_specs:
- filename: microsoft-azure-sql-database-openapi.yml
  format: yaml
  label: Azure SQL Database API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-sql-database/refs/heads/main/openapi/microsoft-azure-sql-database-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Sql Database Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure SQL Database secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure SQL Database
provider_slug: microsoft-azure-sql-database
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-azure-sql-database-openapi.yml
  type: http
slug: microsoft-azure-sql-database-authentication
source_filename: microsoft-azure-sql-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-sql-database-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-azure-sql-database-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-sql-database/refs/heads/main/authentication/microsoft-azure-sql-database-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- SQL
- Relational Database
---
