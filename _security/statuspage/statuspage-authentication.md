---
api_key_in:
- header
api_specs:
- filename: statuspage-webhooks-asyncapi.yml
  format: yaml
  label: Statuspage Webhook Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/statuspage/refs/heads/main/asyncapi/statuspage-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Statuspage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Statuspage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Statuspage
provider_slug: statuspage
scheme_count: 1
schemes:
- description: 'Pass `Authorization: OAuth <api_key>`. The API key may alternatively

    be provided via the `api_key` query parameter.'
  in: header
  name: ApiKey
  parameter: Authorization
  sources:
  - openapi/statuspage-openapi.yml
  type: apiKey
slug: statuspage-authentication
source_filename: statuspage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/statuspage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Pass `Authorization: OAuth <api_key>`. The API key may alternatively\n    be provided via the `api_key` query parameter.\n  sources:\n  - openapi/statuspage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statuspage/refs/heads/main/authentication/statuspage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Status Page
- Incident Communication
- Incident Management
- Uptime
- Reliability
- Atlassian
---
