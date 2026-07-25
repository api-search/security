---
api_key_in:
- header
api_specs:
- filename: tableau-authentication-api-openapi.yml
  format: yaml
  label: Tableau Authentication API
  slug: tableau-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-authentication-api-openapi.yml
- filename: tableau-data-sources-api-openapi.yml
  format: yaml
  label: Tableau Data Sources API
  slug: tableau-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-data-sources-api-openapi.yml
- filename: tableau-favorites-api-openapi.yml
  format: yaml
  label: Tableau Favorites API
  slug: tableau-favorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-favorites-api-openapi.yml
- filename: tableau-groups-api-openapi.yml
  format: yaml
  label: Tableau Groups API
  slug: tableau-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-groups-api-openapi.yml
- filename: tableau-jobs-api-openapi.yml
  format: yaml
  label: Tableau Jobs API
  slug: tableau-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-jobs-api-openapi.yml
- filename: tableau-permissions-api-openapi.yml
  format: yaml
  label: Tableau Permissions API
  slug: tableau-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-permissions-api-openapi.yml
- filename: tableau-projects-api-openapi.yml
  format: yaml
  label: Tableau Projects API
  slug: tableau-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-projects-api-openapi.yml
- filename: tableau-schedules-api-openapi.yml
  format: yaml
  label: Tableau Schedules API
  slug: tableau-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-schedules-api-openapi.yml
- filename: tableau-sites-api-openapi.yml
  format: yaml
  label: Tableau Sites API
  slug: tableau-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-sites-api-openapi.yml
- filename: tableau-subscriptions-api-openapi.yml
  format: yaml
  label: Tableau Subscriptions API
  slug: tableau-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-subscriptions-api-openapi.yml
- filename: tableau-users-api-openapi.yml
  format: yaml
  label: Tableau Users API
  slug: tableau-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-users-api-openapi.yml
- filename: tableau-views-api-openapi.yml
  format: yaml
  label: Tableau Views API
  slug: tableau-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-views-api-openapi.yml
- filename: tableau-workbooks-api-openapi.yml
  format: yaml
  label: Tableau Workbooks API
  slug: tableau-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-workbooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tableau Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tableau secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tableau
provider_slug: tableau
scheme_count: 1
schemes:
- description: The authentication token obtained from the Sign In method. Include this token in the X-Tableau-Auth header of all subsequent requests.
  in: header
  name: TableauAuth
  parameter: X-Tableau-Auth
  sources:
  - openapi/tableau-rest-api-openapi.yml
  type: apiKey
slug: tableau-authentication
source_filename: tableau-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tableau-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TableauAuth\n  type: apiKey\n  in: header\n  parameter: X-Tableau-Auth\n  description: The authentication token obtained from the Sign In method. Include this token\n    in the X-Tableau-Auth header of all subsequent requests.\n  sources:\n  - openapi/tableau-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/authentication/tableau-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
---
