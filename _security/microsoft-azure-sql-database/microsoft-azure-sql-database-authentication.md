---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-sql-database-databases-api-openapi.yml
  format: yaml
  label: Azure SQL Database Databases API
  slug: microsoft-azure-sql-database-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-databases-api-openapi.yml
- filename: microsoft-azure-sql-database-elasticpools-api-openapi.yml
  format: yaml
  label: Azure SQL Database ElasticPools API
  slug: microsoft-azure-sql-database-elasticpools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml
- filename: microsoft-azure-sql-database-failovergroups-api-openapi.yml
  format: yaml
  label: Azure SQL Database FailoverGroups API
  slug: microsoft-azure-sql-database-failovergroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml
- filename: microsoft-azure-sql-database-servers-api-openapi.yml
  format: yaml
  label: Azure SQL Database Servers API
  slug: microsoft-azure-sql-database-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-servers-api-openapi.yml
- filename: microsoft-azure-sql-database-firewall-rules-api-openapi.yml
  format: yaml
  label: Azure SQL Database Firewall Rules API
  slug: microsoft-azure-sql-database-firewall-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Azure Sql Database Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure SQL Database secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure SQL Database
provider_slug: microsoft-azure-sql-database
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-sql-database-databases-api-openapi.yml
  - openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml
  - openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml
  - openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml
  - openapi/microsoft-azure-sql-database-servers-api-openapi.yml
  type: oauth2
slug: microsoft-azure-sql-database-authentication
source_filename: microsoft-azure-sql-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-sql-database-databases-api-openapi.yml, openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml,\n  openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml, openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml,\n  openapi/microsoft-azure-sql-database-servers-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-sql-database-databases-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml\n  - openapi/microsoft-azure-sql-database-servers-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-sql-database/authentication/microsoft-azure-sql-database-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Database
- SQL
- Relational Database
- Microsoft Azure
- Microsoft
- Cloud Database
- Managed Database
- SQL Server
---
