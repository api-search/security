---
api_key_in:
- cookie
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mysql Authentication
name_suffix: Authentication
oauth_flows: []
overview: MySQL secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MySQL
provider_slug: mysql
scheme_count: 2
schemes:
- description: Bearer token obtained from an MRS authentication flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mysql-openapi.yml
  type: http
- description: Session cookie obtained from an MRS authentication flow.
  in: cookie
  name: cookieAuth
  parameter: session_id
  sources:
  - openapi/mysql-openapi.yml
  type: apiKey
slug: mysql-authentication
source_filename: mysql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mysql-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from an MRS authentication flow.\n  sources:\n  - openapi/mysql-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session_id\n  description: Session cookie obtained from an MRS authentication flow.\n  sources:\n  - openapi/mysql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mysql/refs/heads/main/authentication/mysql-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Database
- Open Source
- RDBMS
- Relational Database
- SQL
---
