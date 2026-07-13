---
api_key_in: []
api_specs:
- filename: global-relay-conversation-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Conversation Archiving API
  slug: conversation-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-conversation-archiving-api-openapi.yml
- filename: global-relay-email-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Email Archiving API
  slug: email-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-email-archiving-api-openapi.yml
- filename: global-relay-voice-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Voice Archiving API
  slug: voice-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-voice-archiving-api-openapi.yml
- filename: global-relay-event-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Event Archiving API
  slug: event-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-event-archiving-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Global Relay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Global Relay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Global Relay
provider_slug: global-relay
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Client Credentials grant. Obtain a token from https://iam-oauth2.globalrelay.com/oauth2/token with grant_type=client_credentials and scope=openid conversation.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/global-relay-conversation-archiving-api-openapi.yml
  - openapi/global-relay-email-archiving-api-openapi.yml
  - openapi/global-relay-event-archiving-api-openapi.yml
  - openapi/global-relay-voice-archiving-api-openapi.yml
  type: http
slug: global-relay-authentication
source_filename: global-relay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/global-relay-conversation-archiving-api-openapi.yml, openapi/global-relay-email-archiving-api-openapi.yml,\n  openapi/global-relay-event-archiving-api-openapi.yml, openapi/global-relay-voice-archiving-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Client Credentials grant. Obtain a token from https://iam-oauth2.globalrelay.com/oauth2/token\n    with grant_type=client_credentials and scope=openid conversation.\n  sources:\n  - openapi/global-relay-conversation-archiving-api-openapi.yml\n  - openapi/global-relay-email-archiving-api-openapi.yml\n  - openapi/global-relay-event-archiving-api-openapi.yml\n  - openapi/global-relay-voice-archiving-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/authentication/global-relay-authentication.yml
summary_line: http · 1 scheme
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
---
