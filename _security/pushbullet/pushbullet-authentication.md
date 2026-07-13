---
api_key_in:
- header
api_specs:
- filename: pushbullet-openapi.yml
  format: yaml
  label: Pushbullet HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-openapi.yml
- filename: pushbullet-asyncapi.yml
  format: yaml
  label: Pushbullet Realtime Event Stream
  slug: realtime-event-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-asyncapi.yml
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
