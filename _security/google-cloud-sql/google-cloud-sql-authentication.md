---
api_key_in: []
api_specs:
- filename: cloud-sql-openapi.yml
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-sql/refs/heads/main/openapi/cloud-sql-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Sql Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud SQL secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud SQL
provider_slug: google-cloud-sql
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/cloud-sql-openapi.yml
  type: oauth2
slug: google-cloud-sql-authentication
source_filename: google-cloud-sql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-sql-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/cloud-sql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-sql/refs/heads/main/authentication/google-cloud-sql-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Database
- Google Cloud
- MySQL
- PostgreSQL
- Relational
- SQL
---
