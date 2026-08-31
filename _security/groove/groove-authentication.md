---
api_key_in:
- query
api_specs:
- filename: groove-webhooks-asyncapi.yml
  format: yaml
  label: Groove Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/asyncapi/groove-webhooks-asyncapi.yml
- filename: groove-agents-api-openapi.yml
  format: yaml
  label: Groove Agents API
  slug: groove-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-agents-api-openapi.yml
- filename: groove-attachments-api-openapi.yml
  format: yaml
  label: Groove Attachments API
  slug: groove-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-attachments-api-openapi.yml
- filename: groove-customers-api-openapi.yml
  format: yaml
  label: Groove Customers API
  slug: groove-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-customers-api-openapi.yml
- filename: groove-folders-api-openapi.yml
  format: yaml
  label: Groove Folders API
  slug: groove-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-folders-api-openapi.yml
- filename: groove-groups-api-openapi.yml
  format: yaml
  label: Groove Groups API
  slug: groove-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-groups-api-openapi.yml
- filename: groove-mailboxes-api-openapi.yml
  format: yaml
  label: Groove Mailboxes API
  slug: groove-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-mailboxes-api-openapi.yml
- filename: groove-messages-api-openapi.yml
  format: yaml
  label: Groove Messages API
  slug: groove-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-messages-api-openapi.yml
- filename: groove-tickets-api-openapi.yml
  format: yaml
  label: Groove Tickets API
  slug: groove-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-tickets-api-openapi.yml
- filename: groove-webhooks-api-openapi.yml
  format: yaml
  label: Groove Webhooks API
  slug: groove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/openapi/groove-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Groove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groove secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Groove
provider_slug: groove
scheme_count: 2
schemes:
- description: OAuth 2.0 / personal access token via Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/groove-openapi.yml
  type: http
- description: Access token passed as a URL query parameter.
  in: query
  name: accessTokenQuery
  parameter: access_token
  sources:
  - openapi/groove-openapi.yml
  type: apiKey
slug: groove-authentication
source_filename: groove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/groove-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 / personal access token via Authorization header.\n  sources:\n  - openapi/groove-openapi.yml\n- name: accessTokenQuery\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: Access token passed as a URL query parameter.\n  sources:\n  - openapi/groove-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groove/refs/heads/main/authentication/groove-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Customer-Support
- Helpdesk
- Shared Inbox
- Knowledge Base
- Conversations
- Live Chat
---
