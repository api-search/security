---
api_key_in: []
api_specs:
- filename: microsoft-azure-mysql-openapi.yml
  format: yaml
  label: Azure Database for MySQL Flexible Servers API
  slug: azure-database-for-mysql-flexible-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-mysql/refs/heads/main/openapi/microsoft-azure-mysql-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Mysql Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Database for MySQL secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Database for MySQL
provider_slug: microsoft-azure-mysql
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-mysql-openapi.yml
  type: oauth2
slug: microsoft-azure-mysql-authentication
source_filename: microsoft-azure-mysql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-mysql-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-mysql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-mysql/refs/heads/main/authentication/microsoft-azure-mysql-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Database
- Flexible Server
- Managed Database
- MySQL
- Open Source
- Relational Database
---
