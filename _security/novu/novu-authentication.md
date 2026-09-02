---
api_key_in:
- header
api_specs:
- filename: novu-asyncapi.yml
  format: yaml
  label: Novu Inbox / In-App API
  slug: inbox-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/asyncapi/novu-asyncapi.yml
- filename: novu-activity-api-openapi.yml
  format: yaml
  label: Novu Activity API
  slug: novu-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-activity-api-openapi.yml
- filename: novu-channel-connections-api-openapi.yml
  format: yaml
  label: Novu Channel Connections API
  slug: novu-channel-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-channel-connections-api-openapi.yml
- filename: novu-channel-endpoints-api-openapi.yml
  format: yaml
  label: Novu Channel Endpoints API
  slug: novu-channel-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-channel-endpoints-api-openapi.yml
- filename: novu-contexts-api-openapi.yml
  format: yaml
  label: Novu Contexts API
  slug: novu-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-contexts-api-openapi.yml
- filename: novu-domains-api-openapi.yml
  format: yaml
  label: Novu Domains API
  slug: novu-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-domains-api-openapi.yml
- filename: novu-environment-variables-api-openapi.yml
  format: yaml
  label: Novu Environment Variables API
  slug: novu-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-environment-variables-api-openapi.yml
- filename: novu-environments-api-openapi.yml
  format: yaml
  label: Novu Environments API
  slug: novu-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-environments-api-openapi.yml
- filename: novu-events-api-openapi.yml
  format: yaml
  label: Novu Events API
  slug: novu-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-events-api-openapi.yml
- filename: novu-integrations-api-openapi.yml
  format: yaml
  label: Novu Integrations API
  slug: novu-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-integrations-api-openapi.yml
- filename: novu-layouts-api-openapi.yml
  format: yaml
  label: Novu Layouts API
  slug: novu-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-layouts-api-openapi.yml
- filename: novu-messages-api-openapi.yml
  format: yaml
  label: Novu Messages API
  slug: novu-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-messages-api-openapi.yml
- filename: novu-notifications-api-openapi.yml
  format: yaml
  label: Novu Notifications API
  slug: novu-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-notifications-api-openapi.yml
- filename: novu-subscribers-api-openapi.yml
  format: yaml
  label: Novu Subscribers API
  slug: novu-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-subscribers-api-openapi.yml
- filename: novu-topics-api-openapi.yml
  format: yaml
  label: Novu Topics API
  slug: novu-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-topics-api-openapi.yml
- filename: novu-translations-api-openapi.yml
  format: yaml
  label: Novu Translations API
  slug: novu-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-translations-api-openapi.yml
- filename: novu-workflows-api-openapi.yml
  format: yaml
  label: Novu Workflows API
  slug: novu-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-workflows-api-openapi.yml
- filename: novu-webhooks-api-openapi.yml
  format: yaml
  label: Novu Webhooks API
  slug: novu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-webhooks-api-openapi.yml
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
- Notification
- Messaging
- In-App
- Email
- SMS
- Push
- Chat
- Workflows
- Open-Source
- Subscribers
- Topics
- Inbox
- Workflow Orchestration
- Multi-Channel
- Digest
- MCP
- Framework
- React
---
