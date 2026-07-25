---
api_key_in: []
api_specs:
- filename: knock-audiences-api-openapi.yml
  format: yaml
  label: Knock Audiences API
  slug: knock-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-audiences-api-openapi.yml
- filename: knock-bulk-operations-api-openapi.yml
  format: yaml
  label: Knock Bulk operations API
  slug: knock-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-bulk-operations-api-openapi.yml
- filename: knock-channel-data-api-openapi.yml
  format: yaml
  label: Knock Channel data API
  slug: knock-channel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-channel-data-api-openapi.yml
- filename: knock-feeds-api-openapi.yml
  format: yaml
  label: Knock Feeds API
  slug: knock-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-feeds-api-openapi.yml
- filename: knock-guides-api-openapi.yml
  format: yaml
  label: Knock Guides API
  slug: knock-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-guides-api-openapi.yml
- filename: knock-integrations-api-openapi.yml
  format: yaml
  label: Knock Integrations API
  slug: knock-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-integrations-api-openapi.yml
- filename: knock-messages-api-openapi.yml
  format: yaml
  label: Knock Messages API
  slug: knock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-messages-api-openapi.yml
- filename: knock-microsoft-teams-api-openapi.yml
  format: yaml
  label: Knock Microsoft Teams API
  slug: knock-microsoft-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-microsoft-teams-api-openapi.yml
- filename: knock-objects-api-openapi.yml
  format: yaml
  label: Knock Objects API
  slug: knock-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-objects-api-openapi.yml
- filename: knock-preferences-api-openapi.yml
  format: yaml
  label: Knock Preferences API
  slug: knock-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-preferences-api-openapi.yml
- filename: knock-providers-api-openapi.yml
  format: yaml
  label: Knock Providers API
  slug: knock-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-providers-api-openapi.yml
- filename: knock-schedules-api-openapi.yml
  format: yaml
  label: Knock Schedules API
  slug: knock-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-schedules-api-openapi.yml
- filename: knock-slack-api-openapi.yml
  format: yaml
  label: Knock Slack API
  slug: knock-slack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-slack-api-openapi.yml
- filename: knock-subscriptions-api-openapi.yml
  format: yaml
  label: Knock Subscriptions API
  slug: knock-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-subscriptions-api-openapi.yml
- filename: knock-tenants-api-openapi.yml
  format: yaml
  label: Knock Tenants API
  slug: knock-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-tenants-api-openapi.yml
- filename: knock-users-api-openapi.yml
  format: yaml
  label: Knock Users API
  slug: knock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-users-api-openapi.yml
- filename: knock-workflow-recipient-runs-api-openapi.yml
  format: yaml
  label: Knock Workflow recipient runs API
  slug: knock-workflow-recipient-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-workflow-recipient-runs-api-openapi.yml
- filename: knock-workflow-triggers-api-openapi.yml
  format: yaml
  label: Knock Workflow Triggers API
  slug: knock-workflow-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-workflow-triggers-api-openapi.yml
- filename: knock-workflows-api-openapi.yml
  format: yaml
  label: Knock Workflows API
  slug: knock-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/openapi/knock-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knock
provider_slug: knock
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/knock-openapi.json
  type: http
slug: knock-authentication
source_filename: knock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knock-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/knock-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knock/refs/heads/main/authentication/knock-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Email
- SMS
- Push
- Workflows
---
