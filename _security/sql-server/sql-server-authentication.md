---
api_key_in: []
api_specs:
- filename: sql.json
  format: json
  label: SQL Server REST API
  slug: sql-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/sql/resource-manager/Microsoft.Sql/stable/2021-11-01/sql.json
- filename: databases.json
  format: json
  label: Azure SQL Database REST API
  slug: azure-sql-database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/sql/resource-manager/Microsoft.Sql/stable/2021-11-01/databases.json
auth_types:
- sql-login
- windows-integrated
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Sql Server Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Microsoft SQL Server APIs secures its APIs with sql-login, windows-integrated, oauth2, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Microsoft SQL Server APIs
provider_slug: sql-server
scheme_count: 0
schemes: []
slug: sql-server-authentication
source_filename: sql-server-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  https://learn.microsoft.com/en-us/sql/relational-databases/security/choose-an-authentication-mode\n  and https://learn.microsoft.com/en-us/rest/api/azure/ (Azure REST auth). No\n  local OpenAPI present; profile assembled from provider auth documentation.\nnotes: >-\n  SQL Server has two distinct authentication surfaces: (1) the database engine /\n  driver connection layer (SQL logins, Windows/Kerberos, Microsoft Entra ID), and\n  (2) the Azure management REST APIs (Microsoft Entra ID OAuth 2.0 bearer tokens).\nsummary:\n  types: [sql-login, windows-integrated, oauth2, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\nengine_authentication:\n  docs: https://learn.microsoft.com/en-us/sql/relational-databases/security/choose-an-authentication-mode\n  modes:\n  - name: SQL Server authentication\n    description: Username/password logins managed inside the SQL Server instance.\n  - name:\
  \ Windows authentication\n    description: Integrated Windows/Kerberos/NTLM authentication (Windows domains).\n  - name: Microsoft Entra authentication\n    description: >-\n      Microsoft Entra ID (formerly Azure AD) authentication for Azure SQL and\n      Azure Arc-enabled SQL Server — password, integrated, MFA/interactive,\n      service principal, and managed identity.\n    docs: https://learn.microsoft.com/en-us/azure/azure-sql/database/authentication-aad-overview\n  transport_security:\n    tds_encryption: true\n    strict_encryption: TDS 8.0 with TLS 1.3 (SQL Server 2025)\n    mutual_tls: Client certificate authentication supported via Entra / connection encryption.\nmanagement_rest_authentication:\n  docs: https://learn.microsoft.com/en-us/rest/api/azure/\n  scheme:\n    type: oauth2\n    description: Microsoft Entra ID OAuth 2.0 bearer token in the Authorization header.\n    token_endpoint_discovery: https://login.microsoftonline.com/common/.well-known/openid-configuration\n\
  \    flows:\n    - clientCredentials    # service principal\n    - authorizationCode    # delegated user\n    resource: https://management.azure.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sql-server/refs/heads/main/authentication/sql-server-authentication.yml
summary_line: sql-login/windows-integrated/oauth2/mutualTLS · 0 schemes
tags:
- Azure SQL
- Cloud Database
- Data Management
- Database
- Microsoft
- Relational Database
- SQL
---
