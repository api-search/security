---
api_key_in: []
api_specs:
- filename: raygun-applications-api-openapi.yml
  format: yaml
  label: Raygun Applications API
  slug: raygun-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-applications-api-openapi.yml
- filename: raygun-errors-api-openapi.yml
  format: yaml
  label: Raygun Errors API
  slug: raygun-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-errors-api-openapi.yml
- filename: raygun-deployments-api-openapi.yml
  format: yaml
  label: Raygun Deployments API
  slug: raygun-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-deployments-api-openapi.yml
- filename: raygun-source-maps-api-openapi.yml
  format: yaml
  label: Raygun Source Maps API
  slug: raygun-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-source-maps-api-openapi.yml
- filename: raygun-sessions-api-openapi.yml
  format: yaml
  label: Raygun Sessions API
  slug: raygun-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-sessions-api-openapi.yml
- filename: raygun-pages-api-openapi.yml
  format: yaml
  label: Raygun Pages API
  slug: raygun-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-pages-api-openapi.yml
- filename: raygun-customers-api-openapi.yml
  format: yaml
  label: Raygun Customers API
  slug: raygun-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-customers-api-openapi.yml
- filename: raygun-metrics-api-openapi.yml
  format: yaml
  label: Raygun Metrics API
  slug: raygun-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-metrics-api-openapi.yml
- filename: raygun-flutter-symbols-api-openapi.yml
  format: yaml
  label: Raygun Flutter Symbols API
  slug: raygun-flutter-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-flutter-symbols-api-openapi.yml
- filename: raygun-teams-api-openapi.yml
  format: yaml
  label: Raygun Teams API
  slug: raygun-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-teams-api-openapi.yml
- filename: raygun-invitations-api-openapi.yml
  format: yaml
  label: Raygun Invitations API
  slug: raygun-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-invitations-api-openapi.yml
- filename: raygun-plans-api-openapi.yml
  format: yaml
  label: Raygun Plans API
  slug: raygun-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-plans-api-openapi.yml
- filename: raygun-webhooks-asyncapi.yml
  format: yaml
  label: Raygun Outbound Webhooks
  slug: raygun-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Raygun Authentication
name_suffix: Authentication
oauth_flows: []
overview: Raygun secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Raygun
provider_slug: raygun
scheme_count: 1
schemes:
- description: 'Personal Access Token authorization using the Bearer scheme. Example: `Authorization: Bearer {token}`'
  name: personal_access_token
  scheme: bearer
  sources:
  - openapi/raygun-applications-api-openapi.yml
  - openapi/raygun-customers-api-openapi.yml
  - openapi/raygun-deployments-api-openapi.yml
  - openapi/raygun-errors-api-openapi.yml
  - openapi/raygun-flutter-symbols-api-openapi.yml
  - openapi/raygun-invitations-api-openapi.yml
  - openapi/raygun-metrics-api-openapi.yml
  - openapi/raygun-pages-api-openapi.yml
  - openapi/raygun-plans-api-openapi.yml
  - openapi/raygun-public-api-openapi.yml
  - openapi/raygun-sessions-api-openapi.yml
  - openapi/raygun-source-maps-api-openapi.yml
  - openapi/raygun-teams-api-openapi.yml
  type: http
slug: raygun-authentication
source_filename: raygun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/raygun-applications-api-openapi.yml, openapi/raygun-customers-api-openapi.yml,\n  openapi/raygun-deployments-api-openapi.yml, openapi/raygun-errors-api-openapi.yml, openapi/raygun-flutter-symbols-api-openapi.yml,\n  openapi/raygun-invitations-api-openapi.yml, openapi/raygun-metrics-api-openapi.yml, openapi/raygun-pages-api-openapi.yml,\n  openapi/raygun-plans-api-openapi.yml, openapi/raygun-public-api-openapi.yml, openapi/raygun-sessions-api-openapi.yml,\n  openapi/raygun-source-maps-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: personal_access_token\n  type: http\n  scheme: bearer\n  description: 'Personal Access Token authorization using the Bearer scheme. Example: `Authorization:\n    Bearer {token}`'\n  sources:\n  - openapi/raygun-applications-api-openapi.yml\n  - openapi/raygun-customers-api-openapi.yml\n  - openapi/raygun-deployments-api-openapi.yml\n  - openapi/raygun-errors-api-openapi.yml\n\
  \  - openapi/raygun-flutter-symbols-api-openapi.yml\n  - openapi/raygun-invitations-api-openapi.yml\n  - openapi/raygun-metrics-api-openapi.yml\n  - openapi/raygun-pages-api-openapi.yml\n  - openapi/raygun-plans-api-openapi.yml\n  - openapi/raygun-public-api-openapi.yml\n  - openapi/raygun-sessions-api-openapi.yml\n  - openapi/raygun-source-maps-api-openapi.yml\n  - openapi/raygun-teams-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/authentication/raygun-authentication.yml
summary_line: http · 1 scheme
tags:
- Observability
- Crash Reporting
- Real User Monitoring
- Application Performance Monitoring
- Error Tracking
- Errors
- Monitoring
- DevOps
- Source Maps
- Deployments
---
