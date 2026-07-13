---
api_key_in: []
api_specs:
- filename: knock-workflows-api-openapi.yml
  format: yaml
  label: Knock Workflows API
  slug: knock-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-workflows-api-openapi.yml
- filename: knock-users-api-openapi.yml
  format: yaml
  label: Knock Users API
  slug: knock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-users-api-openapi.yml
- filename: knock-messages-api-openapi.yml
  format: yaml
  label: Knock Messages API
  slug: knock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-messages-api-openapi.yml
- filename: knock-objects-api-openapi.yml
  format: yaml
  label: Knock Objects API
  slug: knock-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-objects-api-openapi.yml
- filename: knock-tenants-api-openapi.yml
  format: yaml
  label: Knock Tenants API
  slug: knock-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-tenants-api-openapi.yml
- filename: knock-schedules-api-openapi.yml
  format: yaml
  label: Knock Schedules API
  slug: knock-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-schedules-api-openapi.yml
- filename: knock-audiences-api-openapi.yml
  format: yaml
  label: Knock Audiences API
  slug: knock-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-audiences-api-openapi.yml
- filename: knock-channels-api-openapi.yml
  format: yaml
  label: Knock Channels API
  slug: knock-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-channels-api-openapi.yml
- filename: knock-providers-api-openapi.yml
  format: yaml
  label: Knock Providers API
  slug: knock-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-providers-api-openapi.yml
- filename: knock-integrations-api-openapi.yml
  format: yaml
  label: Knock Integrations API
  slug: knock-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-integrations-api-openapi.yml
- filename: knock-bulk-operations-api-openapi.yml
  format: yaml
  label: Knock Bulk Operations API
  slug: knock-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-bulk-operations-api-openapi.yml
- filename: knock-notify-api-openapi.yml
  format: yaml
  label: Knock Notify API
  slug: knock-notify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-notify-api-openapi.yml
- filename: knock-management-api-openapi.yml
  format: yaml
  label: Knock Management API (mAPI)
  slug: knock-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-management-api-openapi.yml
- filename: knock-webhooks-asyncapi.yml
  format: yaml
  label: Knock Outbound Webhooks
  slug: knock-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/asyncapi/knock-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knock App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knock
provider_slug: knock-app
scheme_count: 1
schemes:
- description: Knock API key as a Bearer token. Use a public key (pk_...) for client-side requests or a secret key (sk_...) for server-side.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/knock-audiences-api-openapi.yml
  - openapi/knock-bulk-operations-api-openapi.yml
  - openapi/knock-channels-api-openapi.yml
  - openapi/knock-integrations-api-openapi.yml
  - openapi/knock-management-api-openapi.yml
  - openapi/knock-messages-api-openapi.yml
  - openapi/knock-notify-api-openapi.yml
  - openapi/knock-objects-api-openapi.yml
  - openapi/knock-providers-api-openapi.yml
  - openapi/knock-schedules-api-openapi.yml
  - openapi/knock-tenants-api-openapi.yml
  - openapi/knock-users-api-openapi.yml
  - openapi/knock-workflows-api-openapi.yml
  type: http
slug: knock-app-authentication
source_filename: knock-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knock-audiences-api-openapi.yml, openapi/knock-bulk-operations-api-openapi.yml,\n  openapi/knock-channels-api-openapi.yml, openapi/knock-integrations-api-openapi.yml, openapi/knock-management-api-openapi.yml,\n  openapi/knock-messages-api-openapi.yml, openapi/knock-notify-api-openapi.yml, openapi/knock-objects-api-openapi.yml,\n  openapi/knock-providers-api-openapi.yml, openapi/knock-schedules-api-openapi.yml, openapi/knock-tenants-api-openapi.yml,\n  openapi/knock-users-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Knock API key as a Bearer token. Use a public key (pk_...) for client-side requests\n    or a secret key (sk_...) for server-side.\n  sources:\n  - openapi/knock-audiences-api-openapi.yml\n  - openapi/knock-bulk-operations-api-openapi.yml\n  - openapi/knock-channels-api-openapi.yml\n  - openapi/knock-integrations-api-openapi.yml\n\
  \  - openapi/knock-management-api-openapi.yml\n  - openapi/knock-messages-api-openapi.yml\n  - openapi/knock-notify-api-openapi.yml\n  - openapi/knock-objects-api-openapi.yml\n  - openapi/knock-providers-api-openapi.yml\n  - openapi/knock-schedules-api-openapi.yml\n  - openapi/knock-tenants-api-openapi.yml\n  - openapi/knock-users-api-openapi.yml\n  - openapi/knock-workflows-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/authentication/knock-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Messaging
- Infrastructure
- Workflows
- Cross-Channel
- Email
- SMS
- Push
- In-App
- Chat
- Slack
- Webhooks
- MCP
- AI Agents
- Developer Platform
---
