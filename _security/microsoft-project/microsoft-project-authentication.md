---
api_key_in: []
api_specs:
- filename: microsoft-project-assignments-api-openapi.yml
  format: yaml
  label: Microsoft Project Assignments API
  slug: microsoft-project-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-assignments-api-openapi.yml
- filename: microsoft-project-calendars-api-openapi.yml
  format: yaml
  label: Microsoft Project Calendars API
  slug: microsoft-project-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-calendars-api-openapi.yml
- filename: microsoft-project-custom-fields-api-openapi.yml
  format: yaml
  label: Microsoft Project Custom Fields API
  slug: microsoft-project-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-custom-fields-api-openapi.yml
- filename: microsoft-project-enterprise-project-types-api-openapi.yml
  format: yaml
  label: Microsoft Project Enterprise Project Types API
  slug: microsoft-project-enterprise-project-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-enterprise-project-types-api-openapi.yml
- filename: microsoft-project-event-handlers-api-openapi.yml
  format: yaml
  label: Microsoft Project Event Handlers API
  slug: microsoft-project-event-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-event-handlers-api-openapi.yml
- filename: microsoft-project-lookup-tables-api-openapi.yml
  format: yaml
  label: Microsoft Project Lookup Tables API
  slug: microsoft-project-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-lookup-tables-api-openapi.yml
- filename: microsoft-project-phases-api-openapi.yml
  format: yaml
  label: Microsoft Project Phases API
  slug: microsoft-project-phases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-phases-api-openapi.yml
- filename: microsoft-project-projects-api-openapi.yml
  format: yaml
  label: Microsoft Project Projects API
  slug: microsoft-project-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-projects-api-openapi.yml
- filename: microsoft-project-resources-api-openapi.yml
  format: yaml
  label: Microsoft Project Resources API
  slug: microsoft-project-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-resources-api-openapi.yml
- filename: microsoft-project-stages-api-openapi.yml
  format: yaml
  label: Microsoft Project Stages API
  slug: microsoft-project-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-stages-api-openapi.yml
- filename: microsoft-project-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Project Tasks API
  slug: microsoft-project-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-tasks-api-openapi.yml
- filename: microsoft-project-timesheets-api-openapi.yml
  format: yaml
  label: Microsoft Project Timesheets API
  slug: microsoft-project-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-timesheets-api-openapi.yml
- filename: microsoft-project-workflow-activities-api-openapi.yml
  format: yaml
  label: Microsoft Project Workflow Activities API
  slug: microsoft-project-workflow-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-workflow-activities-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Project Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Project secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Project
provider_slug: microsoft-project
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication via Azure AD for SharePoint Online
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: oauth2
  sources:
  - openapi/microsoft-project-rest-api.yaml
  type: oauth2
slug: microsoft-project-authentication
source_filename: microsoft-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-project-rest-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 authentication via Azure AD for SharePoint Online\n  sources:\n  - openapi/microsoft-project-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/authentication/microsoft-project-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio-Management
- Project Management
- Resource Management
- Scheduling
- Task Management
---
