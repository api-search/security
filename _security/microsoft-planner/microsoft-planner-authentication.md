---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-planner-groups-plannergroup-api-openapi.yml
  format: yaml
  label: Microsoft Planner Groups.planner Group API
  slug: microsoft-planner-groups-plannergroup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-groups-plannergroup-api-openapi.yml
- filename: microsoft-planner-me-planneruser-api-openapi.yml
  format: yaml
  label: Microsoft Planner Me.planner User API
  slug: microsoft-planner-me-planneruser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-me-planneruser-api-openapi.yml
- filename: microsoft-planner-planner-planner-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner API
  slug: microsoft-planner-planner-planner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-planner-api-openapi.yml
- filename: microsoft-planner-planner-plannerbucket-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Bucket API
  slug: microsoft-planner-planner-plannerbucket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannerbucket-api-openapi.yml
- filename: microsoft-planner-planner-plannerplan-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Plan API
  slug: microsoft-planner-planner-plannerplan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannerplan-api-openapi.yml
- filename: microsoft-planner-planner-plannertask-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Task API
  slug: microsoft-planner-planner-plannertask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannertask-api-openapi.yml
- filename: microsoft-planner-users-planneruser-api-openapi.yml
  format: yaml
  label: Microsoft Planner Users.planner User API
  slug: microsoft-planner-users-planneruser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-users-planneruser-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Planner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Planner secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Planner
provider_slug: microsoft-planner
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization with Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/_superseded/microsoft-planner-buckets-api-openapi.yml
  - openapi/_superseded/microsoft-planner-plan-details-api-openapi.yml
  - openapi/_superseded/microsoft-planner-plans-api-openapi.yml
  - openapi/_superseded/microsoft-planner-task-details-api-openapi.yml
  - openapi/_superseded/microsoft-planner-tasks-api-openapi.yml
  type: oauth2
slug: microsoft-planner-authentication
source_filename: microsoft-planner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-planner-buckets-api-openapi.yml, openapi/_superseded/microsoft-planner-plan-details-api-openapi.yml,\n  openapi/_superseded/microsoft-planner-plans-api-openapi.yml, openapi/_superseded/microsoft-planner-task-details-api-openapi.yml,\n  openapi/_superseded/microsoft-planner-tasks-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 6\n  description: OAuth 2.0 authorization with Microsoft identity platform\n  sources:\n  - openapi/_superseded/microsoft-planner-buckets-api-openapi.yml\n  - openapi/_superseded/microsoft-planner-plan-details-api-openapi.yml\n  - openapi/_superseded/microsoft-planner-plans-api-openapi.yml\n\
  \  - openapi/_superseded/microsoft-planner-task-details-api-openapi.yml\n  - openapi/_superseded/microsoft-planner-tasks-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-planner/authentication/microsoft-planner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
---
