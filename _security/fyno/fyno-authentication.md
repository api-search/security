---
api_key_in: []
api_specs:
- filename: fyno-fire-an-event-api-openapi.yml
  format: yaml
  label: Fyno Fire an Event API
  slug: fyno-fire-an-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-fire-an-event-api-openapi.yml
- filename: fyno-fyno-verify-api-openapi.yml
  format: yaml
  label: Fyno Fyno Verify API
  slug: fyno-fyno-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-fyno-verify-api-openapi.yml
- filename: fyno-manage-user-profiles-api-openapi.yml
  format: yaml
  label: Fyno Manage User Profiles API
  slug: fyno-manage-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-manage-user-profiles-api-openapi.yml
- filename: fyno-manage-user-subscriptions-preferences-api-openapi.yml
  format: yaml
  label: Fyno Manage User Subscriptions & Preferences API
  slug: fyno-manage-user-subscriptions-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-manage-user-subscriptions-preferences-api-openapi.yml
- filename: fyno-suppression-list-api-openapi.yml
  format: yaml
  label: Fyno Suppression List API
  slug: fyno-suppression-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-suppression-list-api-openapi.yml
- filename: fyno-user-properties-api-openapi.yml
  format: yaml
  label: Fyno User Properties API
  slug: fyno-user-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/openapi/fyno-user-properties-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fyno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fyno secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fyno
provider_slug: fyno
scheme_count: 1
schemes:
- description: Enter your API Key. If you don't have it already, you can create one from the API Keys page within your Fyno account
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fyno-notification-events-openapi.yml
  type: http
slug: fyno-authentication
source_filename: fyno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fyno-notification-events-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Enter your API Key. If you don't have it already, you can create one from the\n    API Keys page within your Fyno account\n  sources:\n  - openapi/fyno-notification-events-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyno/refs/heads/main/authentication/fyno-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Messaging
- Communication
- Push Notifications
- Email
- SMS
- WhatsApp
- In-App
- Orchestration
- Multi-Channel
---
