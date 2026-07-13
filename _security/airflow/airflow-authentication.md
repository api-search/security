---
api_key_in: []
api_specs:
- filename: airflow-openapi.yml
  format: yaml
  label: Apache Airflow API
  slug: airflow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/openapi/airflow-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Airflow Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Apache Airflow secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Apache Airflow
provider_slug: airflow
scheme_count: 2
schemes:
- description: 'To authenticate Airflow API requests, clients must include a JWT (JSON Web Token) in the Authorization header of each request. This token is used to verify the identity of the client and ensure that they have the appropriate permissions to access the requested resources. You can use the endpoint ``POST /auth/token`` in order to generate a JWT token. Upon successful authentication, the server will '
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /auth/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/airflow-openapi.yml
  type: oauth2
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/airflow-openapi.yml
  type: http
slug: airflow-authentication
source_filename: airflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airflow-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /auth/token\n    scopes: 0\n  description: 'To authenticate Airflow API requests, clients must include a JWT (JSON Web Token)\n    in the Authorization header of each request. This token is used to verify the identity of\n    the client and ensure that they have the appropriate permissions to access the requested\n    resources. You can use the endpoint ``POST /auth/token`` in order to generate a JWT token.\n    Upon successful authentication, the server will '\n  sources:\n  - openapi/airflow-openapi.yml\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/airflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/authentication/airflow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
---
