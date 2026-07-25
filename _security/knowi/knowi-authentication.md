---
api_key_in:
- header
api_specs:
- filename: knowi-authentication-api-openapi.yml
  format: yaml
  label: Knowi Authentication API
  slug: knowi-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-authentication-api-openapi.yml
- filename: knowi-dashboards-api-openapi.yml
  format: yaml
  label: Knowi Dashboards API
  slug: knowi-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-dashboards-api-openapi.yml
- filename: knowi-groups-api-openapi.yml
  format: yaml
  label: Knowi Groups API
  slug: knowi-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-groups-api-openapi.yml
- filename: knowi-pull-api-openapi.yml
  format: yaml
  label: Knowi Pull API
  slug: knowi-pull-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-pull-api-openapi.yml
- filename: knowi-push-api-openapi.yml
  format: yaml
  label: Knowi Push API
  slug: knowi-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-push-api-openapi.yml
- filename: knowi-users-api-openapi.yml
  format: yaml
  label: Knowi Users API
  slug: knowi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/authentication/knowi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Analytics
- API Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- NoSQL Analytics
---
