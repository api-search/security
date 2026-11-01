---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agencyzoom-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom Authentication API
  slug: agencyzoom-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-authentication-api-openapi.yml
- filename: agencyzoom-business-classifications-api-openapi.yml
  format: yaml
  label: AgencyZoom Business Classifications API
  slug: agencyzoom-business-classifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-business-classifications-api-openapi.yml
- filename: agencyzoom-configuration-and-settings-api-openapi.yml
  format: yaml
  label: AgencyZoom Configuration and Settings API
  slug: agencyzoom-configuration-and-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-configuration-and-settings-api-openapi.yml
- filename: agencyzoom-contact-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Contact Management API
  slug: agencyzoom-contact-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-contact-management-api-openapi.yml
- filename: agencyzoom-customer-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Customer Management API
  slug: agencyzoom-customer-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-customer-management-api-openapi.yml
- filename: agencyzoom-dashboard-api-openapi.yml
  format: yaml
  label: AgencyZoom Dashboard API
  slug: agencyzoom-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-dashboard-api-openapi.yml
- filename: agencyzoom-department-and-groups-api-openapi.yml
  format: yaml
  label: AgencyZoom Department and Groups API
  slug: agencyzoom-department-and-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-department-and-groups-api-openapi.yml
- filename: agencyzoom-lead-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Lead Management API
  slug: agencyzoom-lead-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-lead-management-api-openapi.yml
- filename: agencyzoom-life-and-health-lead-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Life and Health Lead Management API
  slug: agencyzoom-life-and-health-lead-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-life-and-health-lead-management-api-openapi.yml
- filename: agencyzoom-opportunity-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Opportunity Management API
  slug: agencyzoom-opportunity-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-opportunity-management-api-openapi.yml
- filename: agencyzoom-pipeline-api-openapi.yml
  format: yaml
  label: AgencyZoom Pipeline API
  slug: agencyzoom-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-pipeline-api-openapi.yml
- filename: agencyzoom-service-center-api-openapi.yml
  format: yaml
  label: AgencyZoom Service Center API
  slug: agencyzoom-service-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-service-center-api-openapi.yml
- filename: agencyzoom-task-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Task Management API
  slug: agencyzoom-task-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-task-management-api-openapi.yml
- filename: agencyzoom-thread-api-openapi.yml
  format: yaml
  label: AgencyZoom Thread API
  slug: agencyzoom-thread-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-thread-api-openapi.yml
- filename: agencyzoom-user-management-api-openapi.yml
  format: yaml
  label: AgencyZoom User Management API
  slug: agencyzoom-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-user-management-api-openapi.yml
- filename: agencyzoom-v4sso-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom V4SSO Authentication API
  slug: agencyzoom-v4sso-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-v4sso-authentication-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agencyzoom Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgencyZoom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgencyZoom
provider_slug: agencyzoom
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Login via /v1/api/auth/login or /v1/api/auth/ssologin to obtain a JWT, then send as Authorization Bearer.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/agencyzoom-openapi.yml
  type: http
slug: agencyzoom-authentication
source_filename: agencyzoom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agencyzoom-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Login via /v1/api/auth/login or /v1/api/auth/ssologin to obtain a JWT, then send\n    as Authorization Bearer.\n  sources:\n  - openapi/agencyzoom-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/agencyzoom/authentication/agencyzoom-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- CRM
- Sales Automation
- Agency Management
- Customer Retention
---
