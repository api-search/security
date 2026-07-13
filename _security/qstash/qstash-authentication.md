---
api_key_in: []
api_specs:
- filename: qstash-api-openapi.yml
  format: yaml
  label: QStash API
  slug: qstash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-api-openapi.yml
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
- Webhooks
- Dead Letter Queue
- CRON
- Upstash
---
