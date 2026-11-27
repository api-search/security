---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-cloud-sql-databases-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Databases API
  slug: google-cloud-sql-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-databases-api-openapi.yml
- filename: google-cloud-sql-instances-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Instances API
  slug: google-cloud-sql-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-instances-api-openapi.yml
- filename: google-cloud-sql-users-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Users API
  slug: google-cloud-sql-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-users-api-openapi.yml
- filename: google-cloud-sql-backups-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Backups API
  slug: google-cloud-sql-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-backups-api-openapi.yml
- filename: google-cloud-sql-connect-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Connect API
  slug: google-cloud-sql-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-connect-api-openapi.yml
- filename: google-cloud-sql-flags-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Flags API
  slug: google-cloud-sql-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-flags-api-openapi.yml
- filename: google-cloud-sql-operations-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Operations API
  slug: google-cloud-sql-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-operations-api-openapi.yml
- filename: google-cloud-sql-projects-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Projects API
  slug: google-cloud-sql-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-projects-api-openapi.yml
- filename: google-cloud-sql-tiers-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Cloud Sql Tiers API
  slug: google-cloud-sql-tiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-tiers-api-openapi.yml
- filename: google-cloud-sql-backupruns-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Backup Runs API
  slug: google-cloud-sql-backupruns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-backupruns-api-openapi.yml
- filename: google-cloud-sql-bluegreendeployments-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Blue Green Deployments API
  slug: google-cloud-sql-bluegreendeployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-bluegreendeployments-api-openapi.yml
- filename: google-cloud-sql-sslcerts-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Ssl Certs API
  slug: google-cloud-sql-sslcerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-sslcerts-api-openapi.yml
- filename: google-cloud-sql-workloadcaptures-api-openapi.yml
  format: yaml
  label: Google Cloud SQL Workload Captures API
  slug: google-cloud-sql-workloadcaptures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-sql/openapi/google-cloud-sql-workloadcaptures-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Cloud SQL Authentication
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
source_yaml_url: https://artifacts.apis.io/google-cloud-sql/authentication/google-cloud-sql-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Database
- Google Cloud
- MySQL
- PostgreSQL
- Relational
- SQL
---
