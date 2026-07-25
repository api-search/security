---
api_key_in: []
api_specs:
- filename: inngest-account-api-openapi.yml
  format: yaml
  label: Inngest Account API
  slug: inngest-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-account-api-openapi.yml
- filename: inngest-apps-api-openapi.yml
  format: yaml
  label: Inngest Apps API
  slug: inngest-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-apps-api-openapi.yml
- filename: inngest-environments-api-openapi.yml
  format: yaml
  label: Inngest Environments API
  slug: inngest-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-environments-api-openapi.yml
- filename: inngest-events-api-openapi.yml
  format: yaml
  label: Inngest Events API
  slug: inngest-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-events-api-openapi.yml
- filename: inngest-functions-api-openapi.yml
  format: yaml
  label: Inngest Functions API
  slug: inngest-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-functions-api-openapi.yml
- filename: inngest-keys-api-openapi.yml
  format: yaml
  label: Inngest Keys API
  slug: inngest-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-keys-api-openapi.yml
- filename: inngest-runs-api-openapi.yml
  format: yaml
  label: Inngest Runs API
  slug: inngest-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-runs-api-openapi.yml
- filename: inngest-webhooks-api-openapi.yml
  format: yaml
  label: Inngest Webhooks API
  slug: inngest-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inngest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inngest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inngest
provider_slug: inngest
scheme_count: 1
schemes:
- bearerFormat: signing-key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/inngest-openapi.yml
  type: http
slug: inngest-authentication
source_filename: inngest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inngest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: signing-key\n  sources:\n  - openapi/inngest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/authentication/inngest-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- AgentKit
- Background Jobs
- Connect
- Cron Jobs
- Dev Server
- Durable Endpoints
- Durable Execution
- Event-Driven
- Insights
- Orchestration
- Queues
- Realtime
- Self-Hosting
- Serverless
- Signals
- Step Functions
- Webhooks
- Workflows
---
