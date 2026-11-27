---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-bigquery-analyticshub-organizations-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Organizations API
  slug: google-bigquery-analyticshub-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-organizations-api-openapi.yml
- filename: google-bigquery-analyticshub-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Analyticshub Projects API
  slug: google-bigquery-analyticshub-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-analyticshub-projects-api-openapi.yml
- filename: google-bigquery-bigquery-datasets-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Datasets API
  slug: google-bigquery-bigquery-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-datasets-api-openapi.yml
- filename: google-bigquery-bigquery-jobs-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Jobs API
  slug: google-bigquery-bigquery-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-jobs-api-openapi.yml
- filename: google-bigquery-bigquery-models-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Models API
  slug: google-bigquery-bigquery-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-models-api-openapi.yml
- filename: google-bigquery-bigquery-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Projects API
  slug: google-bigquery-bigquery-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-projects-api-openapi.yml
- filename: google-bigquery-bigquery-routines-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Routines API
  slug: google-bigquery-bigquery-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-routines-api-openapi.yml
- filename: google-bigquery-bigquery-row-access-policies-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Row Access Policies API
  slug: google-bigquery-bigquery-row-access-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-row-access-policies-api-openapi.yml
- filename: google-bigquery-bigquery-tabledata-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tabledata API
  slug: google-bigquery-bigquery-tabledata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tabledata-api-openapi.yml
- filename: google-bigquery-bigquery-tables-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquery Tables API
  slug: google-bigquery-bigquery-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquery-tables-api-openapi.yml
- filename: google-bigquery-bigqueryconnection-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryconnection Projects API
  slug: google-bigquery-bigqueryconnection-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryconnection-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatapolicy Projects API
  slug: google-bigquery-bigquerydatapolicy-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatapolicy-projects-api-openapi.yml
- filename: google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigquerydatatransfer Projects API
  slug: google-bigquery-bigquerydatatransfer-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigquerydatatransfer-projects-api-openapi.yml
- filename: google-bigquery-bigqueryreservation-projects-api-openapi.yml
  format: yaml
  label: Google BigQuery Bigquery Bigqueryreservation Projects API
  slug: google-bigquery-bigqueryreservation-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-bigquery/openapi/google-bigquery-bigqueryreservation-projects-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google BigQuery Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google BigQuery secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google BigQuery
provider_slug: google-bigquery
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/bigquery-api-openapi.yml
  type: oauth2
slug: google-bigquery-authentication
source_filename: google-bigquery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigquery-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/bigquery-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-bigquery/authentication/google-bigquery-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
---
