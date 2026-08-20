---
api_key_in: []
api_specs:
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip Events API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-authentication-api-openapi.yml
  format: yaml
  label: Zulip authentication API
  slug: zulip-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-authentication-api-openapi.yml
- filename: zulip-bots-api-openapi.yml
  format: yaml
  label: Zulip bots API
  slug: zulip-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-bots-api-openapi.yml
- filename: zulip-channels-api-openapi.yml
  format: yaml
  label: Zulip channels API
  slug: zulip-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-channels-api-openapi.yml
- filename: zulip-drafts-api-openapi.yml
  format: yaml
  label: Zulip drafts API
  slug: zulip-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-drafts-api-openapi.yml
- filename: zulip-invites-api-openapi.yml
  format: yaml
  label: Zulip invites API
  slug: zulip-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-invites-api-openapi.yml
- filename: zulip-messages-api-openapi.yml
  format: yaml
  label: Zulip messages API
  slug: zulip-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-messages-api-openapi.yml
- filename: zulip-mobile-api-openapi.yml
  format: yaml
  label: Zulip mobile API
  slug: zulip-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-mobile-api-openapi.yml
- filename: zulip-navigation-views-api-openapi.yml
  format: yaml
  label: Zulip navigation_views API
  slug: zulip-navigation-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-navigation-views-api-openapi.yml
- filename: zulip-real-time-events-api-openapi.yml
  format: yaml
  label: Zulip real_time_events API
  slug: zulip-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-real-time-events-api-openapi.yml
- filename: zulip-reminders-api-openapi.yml
  format: yaml
  label: Zulip reminders API
  slug: zulip-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-reminders-api-openapi.yml
- filename: zulip-scheduled-messages-api-openapi.yml
  format: yaml
  label: Zulip scheduled_messages API
  slug: zulip-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-scheduled-messages-api-openapi.yml
- filename: zulip-server-and-organizations-api-openapi.yml
  format: yaml
  label: Zulip server_and_organizations API
  slug: zulip-server-and-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-server-and-organizations-api-openapi.yml
- filename: zulip-users-api-openapi.yml
  format: yaml
  label: Zulip users API
  slug: zulip-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-users-api-openapi.yml
- filename: zulip-webhooks-api-openapi.yml
  format: yaml
  label: Zulip webhooks API
  slug: zulip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zulip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zulip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zulip
provider_slug: zulip
scheme_count: 1
schemes:
- description: 'Basic authentication, with the user''s email as the username, and the API

    key as the password. The API key can be fetched using the

    `/fetch_api_key` or `/dev_fetch_api_key` endpoints.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/zulip-openapi.yml
  type: http
slug: zulip-authentication
source_filename: zulip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zulip-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic authentication, with the user's email as the username, and the API\n    key as the password. The API key can be fetched using the\n    `/fetch_api_key` or `/dev_fetch_api_key` endpoints.\n  sources:\n  - openapi/zulip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/authentication/zulip-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Messaging
- Team Chat
- Webhook
---
