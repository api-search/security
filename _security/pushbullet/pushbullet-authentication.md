---
api_key_in:
- header
api_specs:
- filename: pushbullet-asyncapi.yml
  format: yaml
  label: Pushbullet Realtime Event Stream
  slug: realtime-event-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-asyncapi.yml
- filename: pushbullet-channels-api-openapi.yml
  format: yaml
  label: Pushbullet Channels API
  slug: pushbullet-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-channels-api-openapi.yml
- filename: pushbullet-chats-api-openapi.yml
  format: yaml
  label: Pushbullet Chats API
  slug: pushbullet-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-chats-api-openapi.yml
- filename: pushbullet-devices-api-openapi.yml
  format: yaml
  label: Pushbullet Devices API
  slug: pushbullet-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-devices-api-openapi.yml
- filename: pushbullet-ephemerals-api-openapi.yml
  format: yaml
  label: Pushbullet Ephemerals API
  slug: pushbullet-ephemerals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-ephemerals-api-openapi.yml
- filename: pushbullet-pushes-api-openapi.yml
  format: yaml
  label: Pushbullet Pushes API
  slug: pushbullet-pushes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-pushes-api-openapi.yml
- filename: pushbullet-subscriptions-api-openapi.yml
  format: yaml
  label: Pushbullet Subscriptions API
  slug: pushbullet-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-subscriptions-api-openapi.yml
- filename: pushbullet-texts-api-openapi.yml
  format: yaml
  label: Pushbullet Texts API
  slug: pushbullet-texts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-texts-api-openapi.yml
- filename: pushbullet-upload-api-openapi.yml
  format: yaml
  label: Pushbullet Upload API
  slug: pushbullet-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-upload-api-openapi.yml
- filename: pushbullet-users-api-openapi.yml
  format: yaml
  label: Pushbullet Users API
  slug: pushbullet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pushbullet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pushbullet secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pushbullet
provider_slug: pushbullet
scheme_count: 2
schemes:
- description: Pushbullet account access token from https://www.pushbullet.com/#settings/account
  in: header
  name: accessToken
  parameter: Access-Token
  sources:
  - openapi/pushbullet-openapi.yml
  type: apiKey
- description: OAuth 2.0 for third-party applications.
  flows:
  - authorizationUrl: https://www.pushbullet.com/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.pushbullet.com/oauth2/token
  name: oauth2
  sources:
  - openapi/pushbullet-openapi.yml
  type: oauth2
slug: pushbullet-authentication
source_filename: pushbullet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pushbullet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: Pushbullet account access token from https://www.pushbullet.com/#settings/account\n  sources:\n  - openapi/pushbullet-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.pushbullet.com/authorize\n    tokenUrl: https://api.pushbullet.com/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 for third-party applications.\n  sources:\n  - openapi/pushbullet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/authentication/pushbullet-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Notifications
- Messaging
- Push Notifications
- Device Sync
- SMS
- File Transfer
---
