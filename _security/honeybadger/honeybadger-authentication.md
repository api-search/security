---
api_key_in:
- header
api_specs:
- filename: honeybadger-webhooks-asyncapi.yml
  format: yaml
  label: Honeybadger Outbound Webhook Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybadger/refs/heads/main/asyncapi/honeybadger-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Honeybadger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Honeybadger secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Honeybadger
provider_slug: honeybadger
scheme_count: 2
schemes:
- description: 'HTTP Basic auth. Use your personal AUTH_TOKEN as the username and

    leave the password empty: `-u AUTH_TOKEN:`. Required for the

    Data API (`/v2/*`).'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/honeybadger-openapi.yml
  type: http
- description: Project API key used by the Reporting API (`/v1/*`).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/honeybadger-openapi.yml
  type: apiKey
slug: honeybadger-authentication
source_filename: honeybadger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/honeybadger-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth. Use your personal AUTH_TOKEN as the username and\n    leave the password empty: `-u AUTH_TOKEN:`. Required for the\n    Data API (`/v2/*`).\n  sources:\n  - openapi/honeybadger-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Project API key used by the Reporting API (`/v1/*`).\n  sources:\n  - openapi/honeybadger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeybadger/refs/heads/main/authentication/honeybadger-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Error Monitoring
- Exception Tracking
- Application Performance Monitoring
- Uptime Monitoring
- Cron Monitoring
- Observability
---
