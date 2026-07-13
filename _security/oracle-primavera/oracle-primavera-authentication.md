---
api_key_in: []
api_specs:
- filename: oracle-primavera-p6-eppm-openapi.yml
  format: yaml
  label: Oracle Primavera P6 EPPM REST API
  slug: oracle-primavera-p6-eppm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-primavera/refs/heads/main/openapi/oracle-primavera-p6-eppm-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Primavera Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Oracle Primavera secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Oracle Primavera
provider_slug: oracle-primavera
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with P6 username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-primavera-p6-eppm-openapi.yml
  type: http
- description: Oracle Identity Cloud Service OAuth2
  flows:
  - authorizationUrl: https://identity.oraclecloud.com/oauth2/v1/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/oracle-primavera-p6-eppm-openapi.yml
  type: oauth2
slug: oracle-primavera-authentication
source_filename: oracle-primavera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-primavera-p6-eppm-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with P6 username and password\n  sources:\n  - openapi/oracle-primavera-p6-eppm-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.oraclecloud.com/oauth2/v1/authorize\n    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token\n    scopes: 2\n  description: Oracle Identity Cloud Service OAuth2\n  sources:\n  - openapi/oracle-primavera-p6-eppm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-primavera/refs/heads/main/authentication/oracle-primavera-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Construction
- Engineering
- Project Management
- Scheduling
- Portfolio Management
- Oracle
---
