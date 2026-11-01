---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: knowi-authentication-api-openapi.yml
  format: yaml
  label: Knowi Authentication API
  slug: knowi-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-authentication-api-openapi.yml
- filename: knowi-dashboards-api-openapi.yml
  format: yaml
  label: Knowi Dashboards API
  slug: knowi-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-dashboards-api-openapi.yml
- filename: knowi-groups-api-openapi.yml
  format: yaml
  label: Knowi Groups API
  slug: knowi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-groups-api-openapi.yml
- filename: knowi-pull-api-openapi.yml
  format: yaml
  label: Knowi Pull API
  slug: knowi-pull-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-pull-api-openapi.yml
- filename: knowi-push-api-openapi.yml
  format: yaml
  label: Knowi Push API
  slug: knowi-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-push-api-openapi.yml
- filename: knowi-users-api-openapi.yml
  format: yaml
  label: Knowi Users API
  slug: knowi-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-users-api-openapi.yml
- filename: knowi-action-management-api-api-openapi.yml
  format: yaml
  label: Knowi Action Management API
  slug: knowi-action-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-action-management-api-api-openapi.yml
- filename: knowi-alerts-api-openapi.yml
  format: yaml
  label: Knowi Alerts API
  slug: knowi-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-alerts-api-openapi.yml
- filename: knowi-authentication-management-api-api-openapi.yml
  format: yaml
  label: Knowi Authentication Management API
  slug: knowi-authentication-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-authentication-management-api-api-openapi.yml
- filename: knowi-category-management-api-api-openapi.yml
  format: yaml
  label: Knowi Category Management API
  slug: knowi-category-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-category-management-api-api-openapi.yml
- filename: knowi-datasource-management-api-api-openapi.yml
  format: yaml
  label: Knowi Datasource Management API
  slug: knowi-datasource-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-datasource-management-api-api-openapi.yml
- filename: knowi-group-management-api-api-openapi.yml
  format: yaml
  label: Knowi Group Management API
  slug: knowi-group-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-group-management-api-api-openapi.yml
- filename: knowi-kpi-management-api-api-openapi.yml
  format: yaml
  label: Knowi KPI Management API
  slug: knowi-kpi-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-kpi-management-api-api-openapi.yml
- filename: knowi-natural-language-processing-management-api-api-openapi.yml
  format: yaml
  label: Knowi Natural Language Processing Management API
  slug: knowi-natural-language-processing-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-natural-language-processing-management-api-api-openapi.yml
- filename: knowi-report-management-api-api-openapi.yml
  format: yaml
  label: Knowi Report Management API
  slug: knowi-report-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-report-management-api-api-openapi.yml
- filename: knowi-role-management-api-api-openapi.yml
  format: yaml
  label: Knowi Role Management API
  slug: knowi-role-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-role-management-api-api-openapi.yml
- filename: knowi-user-management-api-api-openapi.yml
  format: yaml
  label: Knowi User Management API
  slug: knowi-user-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-user-management-api-api-openapi.yml
- filename: knowi-data-sources-api-openapi.yml
  format: yaml
  label: Knowi Data Sources API
  slug: knowi-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-data-sources-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Knowi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knowi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Knowi
provider_slug: knowi
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/knowi-management-api-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/knowi-push-data-api-openapi.yml
  type: apiKey
slug: knowi-authentication
source_filename: knowi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knowi-management-api-openapi.yml, openapi/knowi-push-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/knowi-management-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/knowi-push-data-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/knowi/authentication/knowi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Analytics
- API Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- NoSQL Analytics
---
