---
api_key_in: []
api_specs:
- filename: oracle-essbase-application-configuration-api-openapi.yml
  format: yaml
  label: Oracle Essbase Application Configuration API
  slug: oracle-essbase-application-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-application-configuration-api-openapi.yml
- filename: oracle-essbase-applications-api-openapi.yml
  format: yaml
  label: Oracle Essbase Applications API
  slug: oracle-essbase-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-applications-api-openapi.yml
- filename: oracle-essbase-connections-api-openapi.yml
  format: yaml
  label: Oracle Essbase Connections API
  slug: oracle-essbase-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-connections-api-openapi.yml
- filename: oracle-essbase-databases-api-openapi.yml
  format: yaml
  label: Oracle Essbase Databases API
  slug: oracle-essbase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-databases-api-openapi.yml
- filename: oracle-essbase-dimensions-api-openapi.yml
  format: yaml
  label: Oracle Essbase Dimensions API
  slug: oracle-essbase-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-dimensions-api-openapi.yml
- filename: oracle-essbase-files-api-openapi.yml
  format: yaml
  label: Oracle Essbase Files API
  slug: oracle-essbase-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-files-api-openapi.yml
- filename: oracle-essbase-filters-api-openapi.yml
  format: yaml
  label: Oracle Essbase Filters API
  slug: oracle-essbase-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-filters-api-openapi.yml
- filename: oracle-essbase-groups-api-openapi.yml
  format: yaml
  label: Oracle Essbase Groups API
  slug: oracle-essbase-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-groups-api-openapi.yml
- filename: oracle-essbase-jobs-api-openapi.yml
  format: yaml
  label: Oracle Essbase Jobs API
  slug: oracle-essbase-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-jobs-api-openapi.yml
- filename: oracle-essbase-locks-api-openapi.yml
  format: yaml
  label: Oracle Essbase Locks API
  slug: oracle-essbase-locks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-locks-api-openapi.yml
- filename: oracle-essbase-partitions-api-openapi.yml
  format: yaml
  label: Oracle Essbase Partitions API
  slug: oracle-essbase-partitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-partitions-api-openapi.yml
- filename: oracle-essbase-reports-api-openapi.yml
  format: yaml
  label: Oracle Essbase Reports API
  slug: oracle-essbase-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-reports-api-openapi.yml
- filename: oracle-essbase-roles-api-openapi.yml
  format: yaml
  label: Oracle Essbase Roles API
  slug: oracle-essbase-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-roles-api-openapi.yml
- filename: oracle-essbase-scripts-api-openapi.yml
  format: yaml
  label: Oracle Essbase Scripts API
  slug: oracle-essbase-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-scripts-api-openapi.yml
- filename: oracle-essbase-server-api-openapi.yml
  format: yaml
  label: Oracle Essbase Server API
  slug: oracle-essbase-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-server-api-openapi.yml
- filename: oracle-essbase-sessions-api-openapi.yml
  format: yaml
  label: Oracle Essbase Sessions API
  slug: oracle-essbase-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-sessions-api-openapi.yml
- filename: oracle-essbase-user-session-api-openapi.yml
  format: yaml
  label: Oracle Essbase User Session API
  slug: oracle-essbase-user-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-user-session-api-openapi.yml
- filename: oracle-essbase-users-api-openapi.yml
  format: yaml
  label: Oracle Essbase Users API
  slug: oracle-essbase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-users-api-openapi.yml
- filename: oracle-essbase-variables-api-openapi.yml
  format: yaml
  label: Oracle Essbase Variables API
  slug: oracle-essbase-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/openapi/oracle-essbase-variables-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Essbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Essbase secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Essbase
provider_slug: oracle-essbase
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using Essbase username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-essbase-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token authentication for cloud deployments on Oracle Cloud Infrastructure.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oracle-essbase-rest-api-openapi.yml
  type: http
slug: oracle-essbase-authentication
source_filename: oracle-essbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-essbase-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Essbase username and password.\n  sources:\n  - openapi/oracle-essbase-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token authentication for cloud deployments on Oracle Cloud Infrastructure.\n  sources:\n  - openapi/oracle-essbase-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/authentication/oracle-essbase-authentication.yml
summary_line: http · 2 schemes
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
---
