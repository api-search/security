---
api_key_in: []
api_specs:
- filename: matillion-dpc-agents-api-openapi.yml
  format: yaml
  label: Matillion DPC Agents API
  slug: matillion-dpc-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-agents-api-openapi.yml
- filename: matillion-dpc-environments-api-openapi.yml
  format: yaml
  label: Matillion DPC Environments API
  slug: matillion-dpc-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-environments-api-openapi.yml
- filename: matillion-dpc-pipeline-executions-api-openapi.yml
  format: yaml
  label: Matillion DPC Pipeline Executions API
  slug: matillion-dpc-pipeline-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-pipeline-executions-api-openapi.yml
- filename: matillion-dpc-projects-api-openapi.yml
  format: yaml
  label: Matillion DPC Projects API
  slug: matillion-dpc-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-projects-api-openapi.yml
- filename: matillion-dpc-schedules-api-openapi.yml
  format: yaml
  label: Matillion DPC Schedules API
  slug: matillion-dpc-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-schedules-api-openapi.yml
- filename: matillion-etl-groups-projects-api-openapi.yml
  format: yaml
  label: Matillion ETL Groups & Projects API
  slug: matillion-etl-groups-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-groups-projects-api-openapi.yml
- filename: matillion-etl-jobs-runs-api-openapi.yml
  format: yaml
  label: Matillion ETL Jobs & Runs API
  slug: matillion-etl-jobs-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-jobs-runs-api-openapi.yml
- filename: matillion-etl-schedules-api-openapi.yml
  format: yaml
  label: Matillion ETL Schedules API
  slug: matillion-etl-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-schedules-api-openapi.yml
- filename: matillion-etl-tasks-api-openapi.yml
  format: yaml
  label: Matillion ETL Tasks API
  slug: matillion-etl-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-tasks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Matillion Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Matillion secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Matillion
provider_slug: matillion
scheme_count: 2
schemes:
- description: 'Data Productivity Cloud OAuth2 client-credentials flow. Exchange your client id and secret for a Bearer JWT at the token URL, requesting the audience https://api.matillion.com, then send it as Authorization: Bearer <JWT>.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://id.core.matillion.com/oauth/dpc/token
  name: dpc_oauth
  sources:
  - openapi/matillion-openapi.yml
  type: oauth2
- description: Legacy Matillion ETL HTTP Basic auth using a Matillion ETL instance user's credentials.
  name: etl_basic
  scheme: basic
  sources:
  - openapi/matillion-openapi.yml
  type: http
slug: matillion-authentication
source_filename: matillion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/matillion-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: dpc_oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.core.matillion.com/oauth/dpc/token\n    scopes: 0\n  description: 'Data Productivity Cloud OAuth2 client-credentials flow. Exchange your client\n    id and secret for a Bearer JWT at the token URL, requesting the audience https://api.matillion.com,\n    then send it as Authorization: Bearer <JWT>.'\n  sources:\n  - openapi/matillion-openapi.yml\n- name: etl_basic\n  type: http\n  scheme: basic\n  description: Legacy Matillion ETL HTTP Basic auth using a Matillion ETL instance user's credentials.\n  sources:\n  - openapi/matillion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/authentication/matillion-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Data Integration
- ETL
- ELT
- Data Pipeline
- Cloud Data Warehouse
---
