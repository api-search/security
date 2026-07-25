---
api_key_in:
- header
api_specs:
- filename: rollbar-webhooks-asyncapi.yml
  format: yaml
  label: Rollbar Webhooks
  slug: rollbar-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/asyncapi/rollbar-webhooks-asyncapi.yml
- filename: rollbar-access-tokens-api-openapi.yml
  format: yaml
  label: Rollbar Access Tokens API
  slug: rollbar-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-access-tokens-api-openapi.yml
- filename: rollbar-deploys-api-openapi.yml
  format: yaml
  label: Rollbar Deploys API
  slug: rollbar-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-deploys-api-openapi.yml
- filename: rollbar-invites-api-openapi.yml
  format: yaml
  label: Rollbar Invites API
  slug: rollbar-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-invites-api-openapi.yml
- filename: rollbar-items-api-openapi.yml
  format: yaml
  label: Rollbar Items API
  slug: rollbar-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-items-api-openapi.yml
- filename: rollbar-items-metrics-api-openapi.yml
  format: yaml
  label: Rollbar Items Metrics API
  slug: rollbar-items-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-items-metrics-api-openapi.yml
- filename: rollbar-notifications-api-openapi.yml
  format: yaml
  label: Rollbar Notifications API
  slug: rollbar-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-notifications-api-openapi.yml
- filename: rollbar-occurrences-api-openapi.yml
  format: yaml
  label: Rollbar Occurrences API
  slug: rollbar-occurrences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-occurrences-api-openapi.yml
- filename: rollbar-occurrences-metrics-api-openapi.yml
  format: yaml
  label: Rollbar Occurrences Metrics API
  slug: rollbar-occurrences-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-occurrences-metrics-api-openapi.yml
- filename: rollbar-projects-api-openapi.yml
  format: yaml
  label: Rollbar Projects API
  slug: rollbar-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-projects-api-openapi.yml
- filename: rollbar-resolution-time-metrics-api-openapi.yml
  format: yaml
  label: Rollbar Resolution Time Metrics API
  slug: rollbar-resolution-time-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-resolution-time-metrics-api-openapi.yml
- filename: rollbar-rql-jobs-api-openapi.yml
  format: yaml
  label: Rollbar RQL Jobs API
  slug: rollbar-rql-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-rql-jobs-api-openapi.yml
- filename: rollbar-source-maps-api-openapi.yml
  format: yaml
  label: Rollbar Source Maps API
  slug: rollbar-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-source-maps-api-openapi.yml
- filename: rollbar-teams-api-openapi.yml
  format: yaml
  label: Rollbar Teams API
  slug: rollbar-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-teams-api-openapi.yml
- filename: rollbar-users-api-openapi.yml
  format: yaml
  label: Rollbar Users API
  slug: rollbar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rollbar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rollbar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rollbar
provider_slug: rollbar
scheme_count: 1
schemes:
- description: Rollbar access token for authentication. Requires write or post_server_item scope for creating deploys.
  in: header
  name: accessToken
  parameter: X-Rollbar-Access-Token
  sources:
  - openapi/rollbar-deployment-api-openapi.yml
  - openapi/rollbar-metrics-api-openapi.yml
  - openapi/rollbar-rest-api-openapi.yml
  - openapi/rollbar-rql-api-openapi.yml
  type: apiKey
slug: rollbar-authentication
source_filename: rollbar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rollbar-deployment-api-openapi.yml, openapi/rollbar-metrics-api-openapi.yml,\n  openapi/rollbar-rest-api-openapi.yml, openapi/rollbar-rql-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: X-Rollbar-Access-Token\n  description: Rollbar access token for authentication. Requires write or post_server_item scope\n    for creating deploys.\n  sources:\n  - openapi/rollbar-deployment-api-openapi.yml\n  - openapi/rollbar-metrics-api-openapi.yml\n  - openapi/rollbar-rest-api-openapi.yml\n  - openapi/rollbar-rql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/authentication/rollbar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Error Tracking
- Monitoring
- Debugging
- DevOps
- Application Performance
---
