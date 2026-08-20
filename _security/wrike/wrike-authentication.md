---
api_key_in: []
api_specs:
- filename: wrike-access-roles-api-openapi.yml
  format: yaml
  label: Wrike Access Roles API
  slug: wrike-access-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-access-roles-api-openapi.yml
- filename: wrike-accounts-api-openapi.yml
  format: yaml
  label: Wrike Accounts API
  slug: wrike-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-accounts-api-openapi.yml
- filename: wrike-colors-api-openapi.yml
  format: yaml
  label: Wrike Colors API
  slug: wrike-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-colors-api-openapi.yml
- filename: wrike-comments-api-openapi.yml
  format: yaml
  label: Wrike Comments API
  slug: wrike-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-comments-api-openapi.yml
- filename: wrike-contacts-api-openapi.yml
  format: yaml
  label: Wrike Contacts API
  slug: wrike-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-contacts-api-openapi.yml
- filename: wrike-custom-fields-api-openapi.yml
  format: yaml
  label: Wrike Custom Fields API
  slug: wrike-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-custom-fields-api-openapi.yml
- filename: wrike-folders-and-projects-api-openapi.yml
  format: yaml
  label: Wrike Folders And Projects API
  slug: wrike-folders-and-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-folders-and-projects-api-openapi.yml
- filename: wrike-groups-api-openapi.yml
  format: yaml
  label: Wrike Groups API
  slug: wrike-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-groups-api-openapi.yml
- filename: wrike-tasks-api-openapi.yml
  format: yaml
  label: Wrike Tasks API
  slug: wrike-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-tasks-api-openapi.yml
- filename: wrike-time-logs-api-openapi.yml
  format: yaml
  label: Wrike Time Logs API
  slug: wrike-time-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-time-logs-api-openapi.yml
- filename: wrike-users-api-openapi.yml
  format: yaml
  label: Wrike Users API
  slug: wrike-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-users-api-openapi.yml
- filename: wrike-webhooks-api-openapi.yml
  format: yaml
  label: Wrike Webhooks API
  slug: wrike-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-webhooks-api-openapi.yml
- filename: wrike-workflows-api-openapi.yml
  format: yaml
  label: Wrike Workflows API
  slug: wrike-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/openapi/wrike-workflows-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wrike Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wrike secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wrike
provider_slug: wrike
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://www.wrike.com/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://www.wrike.com/oauth2/token
  name: oauth2
  sources:
  - openapi/wrike-openapi.yml
  type: oauth2
- description: Permanent access token (legacy authentication)
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/wrike-openapi.yml
  type: http
slug: wrike-authentication
source_filename: wrike-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wrike-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wrike.com/oauth2/authorize\n    tokenUrl: https://www.wrike.com/oauth2/token\n    scopes: 6\n  description: OAuth 2.0 authorization code flow\n  sources:\n  - openapi/wrike-openapi.yml\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: Permanent access token (legacy authentication)\n  sources:\n  - openapi/wrike-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrike/refs/heads/main/authentication/wrike-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow-Automation
- Task Management
---
