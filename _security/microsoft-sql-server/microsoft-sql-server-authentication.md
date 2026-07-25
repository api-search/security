---
api_key_in: []
api_specs:
- filename: microsoft-sql-server-azure-sql-databases-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Azure SQL Databases API
  slug: microsoft-sql-server-azure-sql-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-azure-sql-databases-api-openapi.yml
- filename: microsoft-sql-server-azure-sql-servers-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Azure SQL Servers API
  slug: microsoft-sql-server-azure-sql-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-azure-sql-servers-api-openapi.yml
- filename: microsoft-sql-server-data-api-builder-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Data API Builder API
  slug: microsoft-sql-server-data-api-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-data-api-builder-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Sql Server Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Microsoft SQL Server secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Microsoft SQL Server
provider_slug: microsoft-sql-server
scheme_count: 1
schemes:
- description: For Azure SQL management endpoints, authenticate via Microsoft Entra ID against https://management.azure.com/.default. Data API Builder endpoints can be configured to use anonymous, EasyAuth, JWT, or Microsoft Entra ID authentication depending on deployment.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-sql-server-openapi.yml
  type: oauth2
slug: microsoft-sql-server-authentication
source_filename: microsoft-sql-server-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-sql-server-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: For Azure SQL management endpoints, authenticate via Microsoft Entra ID against\n    https://management.azure.com/.default. Data API Builder endpoints can be configured to use\n    anonymous, EasyAuth, JWT, or Microsoft Entra ID authentication depending on deployment.\n  sources:\n  - openapi/microsoft-sql-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/authentication/microsoft-sql-server-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Data Management
- Database
- Enterprise
- Relational Database
- SQL
---
