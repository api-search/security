---
api_key_in: []
api_specs:
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Send API
  slug: notificationapi-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Schedule API
  slug: notificationapi-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Users Identify API
  slug: notificationapi-users-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI User Preferences API
  slug: notificationapi-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Notifications Config API
  slug: notificationapi-notifications-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI In-App Inbox API
  slug: notificationapi-in-app-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Logs API
  slug: notificationapi-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notificationapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: NotificationAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NotificationAPI
provider_slug: notificationapi
scheme_count: 1
schemes:
- description: HTTP Basic authentication. For account-level calls the username is your clientId and the password is your clientSecret. Per-user calls (identify user, in-app inbox, delete preferences) use `base64(clientId:userId:hmac)` where hmac is HMAC-SHA256(userId) keyed with the clientSecret.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/notificationapi-openapi.yml
  type: http
slug: notificationapi-authentication
source_filename: notificationapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/notificationapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. For account-level calls the username is your clientId\n    and the password is your clientSecret. Per-user calls (identify user, in-app inbox, delete\n    preferences) use `base64(clientId:userId:hmac)` where hmac is HMAC-SHA256(userId) keyed\n    with the clientSecret.\n  sources:\n  - openapi/notificationapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/authentication/notificationapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Messaging
- Email
- SMS
- Push
- In-App Inbox
---
