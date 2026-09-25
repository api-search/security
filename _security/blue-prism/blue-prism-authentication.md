---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blue-prism-calendars-api-openapi.yml
  format: yaml
  label: Blue Prism Calendars API
  slug: blue-prism-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-calendars-api-openapi.yml
- filename: blue-prism-dashboards-api-openapi.yml
  format: yaml
  label: Blue Prism Dashboards API
  slug: blue-prism-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-dashboards-api-openapi.yml
- filename: blue-prism-encryption-schemes-api-openapi.yml
  format: yaml
  label: Blue Prism Encryption Schemes API
  slug: blue-prism-encryption-schemes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-encryption-schemes-api-openapi.yml
- filename: blue-prism-environment-variables-api-openapi.yml
  format: yaml
  label: Blue Prism Environment Variables API
  slug: blue-prism-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-environment-variables-api-openapi.yml
- filename: blue-prism-health-api-openapi.yml
  format: yaml
  label: Blue Prism Health API
  slug: blue-prism-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-health-api-openapi.yml
- filename: blue-prism-licenses-api-openapi.yml
  format: yaml
  label: Blue Prism Licenses API
  slug: blue-prism-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-licenses-api-openapi.yml
- filename: blue-prism-pools-api-openapi.yml
  format: yaml
  label: Blue Prism Pools API
  slug: blue-prism-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-pools-api-openapi.yml
- filename: blue-prism-processes-api-openapi.yml
  format: yaml
  label: Blue Prism Processes API
  slug: blue-prism-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-processes-api-openapi.yml
- filename: blue-prism-resources-api-openapi.yml
  format: yaml
  label: Blue Prism Resources API
  slug: blue-prism-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-resources-api-openapi.yml
- filename: blue-prism-schedulelogs-api-openapi.yml
  format: yaml
  label: Blue Prism Schedule Logs API
  slug: blue-prism-schedulelogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-schedulelogs-api-openapi.yml
- filename: blue-prism-schedules-api-openapi.yml
  format: yaml
  label: Blue Prism Schedules API
  slug: blue-prism-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-schedules-api-openapi.yml
- filename: blue-prism-sessions-api-openapi.yml
  format: yaml
  label: Blue Prism Sessions API
  slug: blue-prism-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-sessions-api-openapi.yml
- filename: blue-prism-subscriptions-api-openapi.yml
  format: yaml
  label: Blue Prism Subscriptions API
  slug: blue-prism-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-subscriptions-api-openapi.yml
- filename: blue-prism-user-api-openapi.yml
  format: yaml
  label: Blue Prism User API
  slug: blue-prism-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-user-api-openapi.yml
- filename: blue-prism-work-queue-groups-api-openapi.yml
  format: yaml
  label: Blue Prism Work Queue Groups API
  slug: blue-prism-work-queue-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-work-queue-groups-api-openapi.yml
- filename: blue-prism-work-queues-api-openapi.yml
  format: yaml
  label: Blue Prism Work Queues API
  slug: blue-prism-work-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-work-queues-api-openapi.yml
- filename: blue-prism-timezones-api-openapi.yml
  format: yaml
  label: Blue Prism Timezones API
  slug: blue-prism-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-timezones-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Blue Prism Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Blue Prism secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Blue Prism
provider_slug: blue-prism
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token issued from Authentication Server.
  name: Bearer
  scheme: bearer
  sources:
  - openapi/blue-prism-enterprise-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth-server/connect/token
  name: OAuth2
  sources:
  - openapi/blue-prism-enterprise-api-openapi.yml
  type: oauth2
slug: blue-prism-authentication
source_filename: blue-prism-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/blue-prism-enterprise-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token issued from Authentication Server.\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-server/connect/token\n    scopes: 2\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/authentication/blue-prism-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Automation
- RPA
- Intelligent Automation
- Business Process Management
- Process Orchestration
- AI Agents
- Workflow Automation
- Enterprise Software
---
