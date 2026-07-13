---
api_key_in: []
api_specs:
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Planner API
  slug: microsoft-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Plans API
  slug: microsoft-graph-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Tasks API
  slug: microsoft-graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Buckets API
  slug: microsoft-graph-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
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
  - openapi/microsoft-planner-openapi.yml
  type: oauth2
slug: microsoft-planner-authentication
source_filename: microsoft-planner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-planner-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 6\n  description: OAuth 2.0 authorization with Microsoft identity platform\n  sources:\n  - openapi/microsoft-planner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/authentication/microsoft-planner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
---
