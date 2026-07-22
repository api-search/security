---
api_key_in: []
api_specs:
- filename: macroscope-webhook-api.json
  format: json
  label: Macroscope Agent Webhook API
  slug: macroscope-agent-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macroscope/refs/heads/main/openapi/macroscope-webhook-api.json
auth_types: []
description: 'Authentication profile for Macroscope''s agent webhook API. The API uses two distinct credentials at two stages: a per-webhook API key (sent as the X-Webhook-Secret header) to trigger the agent, and a short-lived signed job token (sent as an Authorization: Bearer header) to poll for that one job''s result. There is no OAuth. Keys are created per webhook in the web app.'
kind: authentication
layout: security
method: searched
name: Macroscope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macroscope declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Macroscope
provider_slug: macroscope
scheme_count: 2
schemes:
- description: Per-webhook API key created in Settings -> Connections -> Webhooks. Shown once at creation and cannot be retrieved later. A workspace can have multiple named webhooks each with its own key.
  id: webhookSecret
  in: header
  name: X-Webhook-Secret
  rotation: Create a new webhook to obtain a new key; keys are not re-displayed.
  type: apiKey
  used_by: POST query-agent-webhook-trigger
- bearer_format: JWT
  description: 'Signed token returned by the trigger response (jobToken). Authorizes reads of a single job''s result and is sent as Authorization: Bearer. Valid for about one hour; if it expires before the job finishes, polling returns 403 and the query must be re-triggered for a fresh token.'
  id: jobToken
  scheme: bearer
  scope: single job / single workspace
  type: http
  used_by: GET query-agent-jobs (polling)
slug: macroscope-authentication
source_filename: macroscope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.macroscope.com/api.md\ndocs: https://docs.macroscope.com/api.md\ndescription: >-\n  Authentication profile for Macroscope's agent webhook API. The API uses two\n  distinct credentials at two stages: a per-webhook API key (sent as the\n  X-Webhook-Secret header) to trigger the agent, and a short-lived signed job\n  token (sent as an Authorization: Bearer header) to poll for that one job's\n  result. There is no OAuth. Keys are created per webhook in the web app.\nbase_url: https://hooks.macroscope.com\nschemes:\n  - id: webhookSecret\n    type: apiKey\n    in: header\n    name: X-Webhook-Secret\n    used_by: POST query-agent-webhook-trigger\n    description: >-\n      Per-webhook API key created in Settings -> Connections -> Webhooks. Shown\n      once at creation and cannot be retrieved later. A workspace can have\n      multiple named webhooks each with its own key.\n    rotation: Create a new webhook to obtain\
  \ a new key; keys are not re-displayed.\n  - id: jobToken\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    used_by: GET query-agent-jobs (polling)\n    description: >-\n      Signed token returned by the trigger response (jobToken). Authorizes reads\n      of a single job's result and is sent as Authorization: Bearer. Valid for\n      about one hour; if it expires before the job finishes, polling returns 403\n      and the query must be re-triggered for a fresh token.\n    scope: single job / single workspace\nnotes:\n  - >-\n    External delivery URLs must be allowlisted (Settings -> Connections ->\n    Webhooks -> Allowed External URLs) and must be HTTPS; only GitHub\n    organization admins can manage the list.\n  - >-\n    Product integrations (GitHub, Slack, Jira, Linear, etc.) authenticate via\n    their own OAuth connect flows in Settings -> Connections; those are not part\n    of the public HTTP API surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macroscope/refs/heads/main/authentication/macroscope-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Code Review
- Code Intelligence
- Developer Tools
- Pull Requests
- Agent
- Webhooks
- DevOps
---
