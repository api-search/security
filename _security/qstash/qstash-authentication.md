---
api_key_in: []
api_specs:
- filename: qstash-dead-letter-queue-api-openapi.yml
  format: yaml
  label: QStash Dead Letter Queue API
  slug: qstash-dead-letter-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-dead-letter-queue-api-openapi.yml
- filename: qstash-flow-control-api-openapi.yml
  format: yaml
  label: QStash Flow Control API
  slug: qstash-flow-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-flow-control-api-openapi.yml
- filename: qstash-logs-api-openapi.yml
  format: yaml
  label: QStash Logs API
  slug: qstash-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-logs-api-openapi.yml
- filename: qstash-messages-api-openapi.yml
  format: yaml
  label: QStash Messages API
  slug: qstash-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-messages-api-openapi.yml
- filename: qstash-queues-api-openapi.yml
  format: yaml
  label: QStash Queues API
  slug: qstash-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-queues-api-openapi.yml
- filename: qstash-schedules-api-openapi.yml
  format: yaml
  label: QStash Schedules API
  slug: qstash-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-schedules-api-openapi.yml
- filename: qstash-url-groups-api-openapi.yml
  format: yaml
  label: QStash URL Groups API
  slug: qstash-url-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-url-groups-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qstash Authentication
name_suffix: Authentication
oauth_flows: []
overview: QStash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QStash
provider_slug: qstash
scheme_count: 1
schemes:
- description: Bearer token obtained from the Upstash console at https://console.upstash.com/qstash. Alternatively, pass as query parameter `qstash_token`.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/qstash-api-openapi.yml
  type: http
slug: qstash-authentication
source_filename: qstash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qstash-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the Upstash console at https://console.upstash.com/qstash.\n    Alternatively, pass as query parameter `qstash_token`.\n  sources:\n  - openapi/qstash-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/authentication/qstash-authentication.yml
summary_line: http · 1 scheme
tags:
- Message Queue
- Task Scheduling
- Serverless
- HTTP Messaging
- Background Jobs
- Webhook
- Dead Letter Queue
- Cron
- Upstash
---
