---
api_key_in:
- header
api_specs:
- filename: novu-openapi.yml
  format: yaml
  label: Novu REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-openapi.yml
- filename: novu-openapi.yml
  format: yaml
  label: Novu REST API (EU Region)
  slug: rest-api-eu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-openapi.yml
- filename: novu-asyncapi.yml
  format: yaml
  label: Novu Inbox / In-App API
  slug: inbox-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/asyncapi/novu-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Novu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Novu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Novu
provider_slug: novu
scheme_count: 1
schemes:
- description: 'API key authentication. Allowed headers-- "Authorization: ApiKey <novu_secret_key>".'
  in: header
  name: secretKey
  parameter: Authorization
  sources:
  - openapi/novu-openapi.yml
  type: apiKey
slug: novu-authentication
source_filename: novu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/novu-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: secretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Allowed headers-- \"Authorization: ApiKey <novu_secret_key>\".'\n  sources:\n  - openapi/novu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/authentication/novu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Notifications
- Messaging
- In App
- Email
- SMS
- Push
- Chat
- Workflows
- Open Source
- Subscribers
- Topics
- Inbox
- Workflow Orchestration
- Multi Channel
- Digest
- MCP
- Framework
- React
---
