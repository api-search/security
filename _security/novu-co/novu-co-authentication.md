---
api_key_in:
- header
api_specs:
- filename: novu-co-asyncapi.yml
  format: yaml
  label: Novu Inbox Realtime API
  slug: novu-co-inbox-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/asyncapi/novu-co-asyncapi.yml
- filename: novu-co-environments-api-openapi.yml
  format: yaml
  label: Novu Environments API
  slug: novu-co-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-environments-api-openapi.yml
- filename: novu-co-events-api-openapi.yml
  format: yaml
  label: Novu Events API
  slug: novu-co-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-events-api-openapi.yml
- filename: novu-co-inbox-api-openapi.yml
  format: yaml
  label: Novu Inbox API
  slug: novu-co-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-inbox-api-openapi.yml
- filename: novu-co-integrations-api-openapi.yml
  format: yaml
  label: Novu Integrations API
  slug: novu-co-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-integrations-api-openapi.yml
- filename: novu-co-layouts-api-openapi.yml
  format: yaml
  label: Novu Layouts API
  slug: novu-co-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-layouts-api-openapi.yml
- filename: novu-co-messages-api-openapi.yml
  format: yaml
  label: Novu Messages API
  slug: novu-co-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-messages-api-openapi.yml
- filename: novu-co-notifications-api-openapi.yml
  format: yaml
  label: Novu Notifications API
  slug: novu-co-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-notifications-api-openapi.yml
- filename: novu-co-preferences-api-openapi.yml
  format: yaml
  label: Novu Preferences API
  slug: novu-co-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-preferences-api-openapi.yml
- filename: novu-co-subscribers-api-openapi.yml
  format: yaml
  label: Novu Subscribers API
  slug: novu-co-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-subscribers-api-openapi.yml
- filename: novu-co-topics-api-openapi.yml
  format: yaml
  label: Novu Topics API
  slug: novu-co-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-topics-api-openapi.yml
- filename: novu-co-translations-api-openapi.yml
  format: yaml
  label: Novu Translations API
  slug: novu-co-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-translations-api-openapi.yml
- filename: novu-co-workflows-api-openapi.yml
  format: yaml
  label: Novu Workflows API
  slug: novu-co-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Novu Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Novu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Novu
provider_slug: novu-co
scheme_count: 1
schemes:
- description: 'Novu secret API key from the Dashboard API Keys page, sent as `Authorization: ApiKey <NOVU_SECRET_KEY>`.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/novu-co-openapi.yml
  type: apiKey
slug: novu-co-authentication
source_filename: novu-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/novu-co-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Novu secret API key from the Dashboard API Keys page, sent as `Authorization:\n    ApiKey <NOVU_SECRET_KEY>`.'\n  sources:\n  - openapi/novu-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/authentication/novu-co-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Notifications
- Multi-Channel
- Email
- SMS
- Push
- Chat
- In-App Inbox
- Open Source
- WebSocket
---
