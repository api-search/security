---
api_key_in: []
api_specs:
- filename: oracle-database-19c-ords-openapi.yml
  format: yaml
  label: Oracle REST Data Services (ORDS)
  slug: oracle-rest-data-services-ords
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/refs/heads/main/openapi/oracle-database-19c-ords-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Database 19C Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Oracle Database 19c secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Oracle Database 19c
provider_slug: oracle-database-19c
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-database-19c-ords-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{host}:{port}/ords/{schema}/oauth/token
  name: oauth2
  sources:
  - openapi/oracle-database-19c-ords-openapi.yml
  type: oauth2
slug: oracle-database-19c-authentication
source_filename: oracle-database-19c-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-database-19c-ords-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/oracle-database-19c-ords-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{host}:{port}/ords/{schema}/oauth/token\n    scopes: 0\n  sources:\n  - openapi/oracle-database-19c-ords-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/refs/heads/main/authentication/oracle-database-19c-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Database
- Enterprise
- Json
- Machine-Learning
- Nosql
- Oracle
- Rest
- Sql
---
